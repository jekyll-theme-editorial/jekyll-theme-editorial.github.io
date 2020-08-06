---
title:            "Tempus ullamcorper"
subtitle:
author:           [julia, petunia]
date:             2020-01-03 08:01:02 -0800
last_modified_at: 2020-01-29 19:20:21 -0800
categories:       [jekyll, chortle puffs]
tags:             [tempus, ullamcorper, whizbang]
series:           "build-a-blog"
website:          https://tempus-ullamcorper.example.com/
# NOTE: this post is using the shortcut style for specifying *one* image for 
#       use everywhere related with this post
thumbnail:        pic03-thumb.jpg
image:            pic03.jpg
alt_text:         "I'm an image's alt text, used by screen readers to describe this image."
image_title:      "I'm an image title."
caption:          "I'm an image caption."
excerpt:          "Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam."
---

## Tempus ullamcorpervarius

{:.pullquote data-pullquote="Praesent tempor ligula elementum dui volutpat posuere."}
Tempus ullamcorpervarius purus. Sed sodales sapien at varius interdum. Curabitur ut lacinia turpis. Aliquam egestas euismod erat. Mauris magna sapien, maximus in blandit eget, egestas vitae nisi. Mauris ultrices bibendum velit, at dapibus purus hendrerit id. Praesent ullamcorper finibus mauris, nec gravida enim placerat nec. Praesent tempor ligula elementum dui volutpat posuere.

### Laoreet quis porta
Proin imperdiet, est eget tincidunt convallis, elit velit ultrices massa, ac sollicitudin ligula ligula sed mi. Maecenas sollicitudin tempor urna nec aliquam. Sed ligula purus, suscipit mollis erat rhoncus, eleifend auctor ligula. Quisque quis pulvinar nibh. Nulla aliquam risus non consectetur sollicitudin. Aliquam erat volutpat. Ut euismod turpis ullamcorper neque mollis porttitor. Sed libero massa, ultricies ac augue sit amet, mattis scelerisque tortor. Proin aliquet tellus eget justo pellentesque ultricies. Nulla mollis sem turpis, vel bibendum nibh congue et. Suspendisse lobortis in lacus eget scelerisque. Vestibulum erat nulla, laoreet quis porta ac, tristique in nisl.

<aside class="pullquote"><p>Two options: data-pullquote attribute or aside block.</p></aside>

Mauris quis semper nibh, ac dictum urna. Maecenas ac porta tortor. Suspendisse tincidunt mattis sem et venenatis. Praesent eget est viverra, placerat elit quis, finibus nisi. Pellentesque et ex et quam lobortis mattis. Curabitur vulputate urna nec leo interdum, sed interdum lacus posuere. Praesent at massa quis mauris fermentum iaculis eget in felis. 

### Jekyll's theme.rb
``` ruby
# frozen_string_literal: true

module Jekyll
  class Theme
    extend Forwardable
    attr_reader   :name

    def_delegator :gemspec, :version, :version

    def initialize(name)
      @name = name.downcase.strip
      Jekyll.logger.debug "Theme:", name
      Jekyll.logger.debug "Theme source:", root
    end

    def root
      # Must use File.realpath to resolve symlinks created by rbenv
      # Otherwise, Jekyll.sanitized path with prepend the unresolved root
      @root ||= File.realpath(gemspec.full_gem_path)
    rescue Errno::ENOENT, Errno::EACCES, Errno::ELOOP
      raise "Path #{gemspec.full_gem_path} does not exist, is not accessible "\
        "or includes a symbolic link loop"
    end

    # The name of theme directory
    def basename
      @basename ||= File.basename(root)
    end

    def includes_path
      @includes_path ||= path_for "_includes"
    end

    def layouts_path
      @layouts_path ||= path_for "_layouts"
    end

    def sass_path
      @sass_path ||= path_for "_sass"
    end

    def assets_path
      @assets_path ||= path_for "assets"
    end

    def runtime_dependencies
      gemspec.runtime_dependencies
    end

    private

    def path_for(folder)
      path = realpath_for(folder)
      path if path && File.directory?(path)
    end

    def realpath_for(folder)
      # This resolves all symlinks for the theme subfolder and then ensures that the directory
      # remains inside the theme root. This prevents the use of symlinks for theme subfolders to
      # escape the theme root.
      # However, symlinks are allowed to point to other directories within the theme.
      Jekyll.sanitized_path(root, File.realpath(Jekyll.sanitized_path(root, folder.to_s)))
    rescue Errno::ENOENT, Errno::EACCES, Errno::ELOOP => e
      log_realpath_exception(e, folder)
      nil
    end

    def log_realpath_exception(err, folder)
      return if err.is_a?(Errno::ENOENT)

      case err
      when Errno::EACCES
        Jekyll.logger.error "Theme error:", "Directory '#{folder}' is not accessible."
      when Errno::ELOOP
        Jekyll.logger.error "Theme error:", "Directory '#{folder}' includes a symbolic link loop."
      end
    end

    def gemspec
      @gemspec ||= Gem::Specification.find_by_name(name)
    rescue Gem::LoadError
      raise Jekyll::Errors::MissingDependencyException,
            "The #{name} theme could not be found."
    end
  end
end
```

