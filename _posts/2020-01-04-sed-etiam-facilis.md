---
title:            "Sed etiam facilis"
subtitle:         "when one title won't do, add another!"
author:           augustus
date:             2020-01-04 08:01:02 -0800
last_modified_at: 
categories:       [jekyll, editorial]
tags:             [tempus, sed, facilis, lolligag]
series:           "build-a-blog"
images:
  default:
    file:         pic04.jpg
    alt_text:     "I'm the default image's alt_text for the post 'Sed etiam facilis'."
    title:        "This post, 'Sed etiam facilis', also has a title attribute set for the default image."
# NOTE because of the initial heading, we make the excerpt explicit to exclude the heading.
excerpt:          "Sed etiam facilis semper vehicula ligula. Fusce mattis tortor tortor, id varius diam pellentesque pretium. Integer lobortis tellus sit amet volutpat vestibulum. Aliquam id auctor ante. Aenean tincidunt viverra ipsum vitae commodo. Nam semper vehicula ornare."
---

## Headings make the text
Sed etiam facilis semper vehicula ligula. Fusce mattis tortor tortor, id varius diam pellentesque pretium. Integer lobortis tellus sit amet volutpat vestibulum. Aliquam id auctor ante. Aenean tincidunt viverra ipsum vitae commodo. Nam semper vehicula ornare.

### If something is really important, put it in a box!

{:.box}
Donec sit amet nunc sed erat tempus gravida sit amet nec enim. Sed vehicula lorem urna, sed finibus tortor varius at. Vestibulum nulla diam, vestibulum et nisl eu, venenatis vehicula nulla. Fusce mi nisl, accumsan ac ultrices non, aliquet aliquet velit. Vivamus pellentesque tincidunt lacus, non pharetra orci lacinia at. Donec tempor vestibulum sem vel dictum. Praesent consequat elit vitae massa lacinia, quis cursus ex tempor. Nulla velit nulla, hendrerit sagittis tortor quis, consequat tincidunt tortor. 

Quisque sit amet mollis massa, quis facilisis nulla. Nullam mattis mattis dolor et viverra. Donec vel lacinia purus. Mauris sollicitudin mattis nisi, in pulvinar augue ultricies nec. Aliquam dictum, tortor ut varius consectetur, urna odio vehicula diam, eget venenatis elit eros eget lacus. Suspendisse at euismod magna, a lobortis est. Nunc ac fermentum nibh, a molestie velit. 

### or a blockquote

> Curabitur vel enim felis. Integer auctor purus sit amet dignissim mattis. Proin ultrices erat ut condimentum aliquam. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae;

Nullam gravida, urna eu lacinia volutpat, nibh lorem posuere felis, nec dignissim mauris lectus vel massa. Curabitur lacus felis, aliquam sed nibh vitae, dictum bibendum nulla. In hac habitasse platea dictumst. Ut ultricies viverra diam, nec fringilla mauris vulputate nec. Ut tincidunt pretium tortor, sed elementum ex cursus a. Pellentesque sagittis auctor lectus. Nulla vitae purus non nulla vulputate pellentesque. Nullam id ex et turpis dignissim mollis ornare in erat. Nullam rhoncus nulla eu fringilla sodales. Nam scelerisque mattis risus. Phasellus vitae consequat lectus, quis tempor enim. Donec elementum consequat sodales. Sed ex nunc, facilisis ut urna et, pulvinar ultrices justo. Nullam nec consequat purus, in luctus velit. 

### Here's some HTML all nicely color-coded
```html
<section>
  <div class="row gtr-50 gtr-uniform">
    <div class="col-4">
      <a href="/posts/feugiat-lorem-aenean.html" title="Read 'Feugiat lorem aenean'" class="image">
        <figure class="image fit">
          <img src="/assets/images/pic05-thumb.jpg" alt="this is the default alt text for all images related to the post 'Feugiat lorem aenean'."/>
        </figure>
      </a>
    </div>
    <div class="col-8">
      <header>
        <h3><a href="/posts/feugiat-lorem-aenean.html" title="Read 'Feugiat lorem aenean'">Feugiat lorem aenean</a></h3>
        <p><a href="/people/aurelius.html" rel="author" title="Read Aurelius's bio">Aurelius Maximus</a></p>
      </header>
      <p>Feugiat lorem aenean metus. Maecenas sed orci in dui finibus sodales ut nec nisl. Sed eget luctus nibh, at rhoncus erat. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Etiam at nulla lorem. Integer lorem mi, molestie vel laoreet non, mattis non felis.</p>
    </div>
  </div>
  <hr class="major"/>
  <div class="row gtr-50 gtr-uniform">
    <div class="col-4">
      <a href="/posts/sed-etiam-facilis.html" title="Read 'Sed etiam facilis'" class="image">
        <figure class="image fit">
          <img src="/assets/images/pic04.jpg" alt="I'm the default image's alt_text for the post 'Sed etiam facilis'."/>
        </figure>
      </a>
    </div>
    <div class="col-8">
      <header>
        <h3><a href="/posts/sed-etiam-facilis.html" title="Read 'Sed etiam facilis'">Sed etiam facilis</a></h3>
        <p><a href="/people/augustus.html" rel="author" title="Read Augustus's bio">Augustus Minimus</a></p>
      </header>
      <p>Sed etiam facilis semper vehicula ligula. Fusce mattis tortor tortor, id varius diam pellentesque pretium. Integer lobortis tellus sit amet volutpat vestibulum. Aliquam id auctor ante. Aenean tincidunt viverra ipsum vitae commodo. Nam semper vehicula ornare.</p>
    </div>
  </div>
</section>
```