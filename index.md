---
layout:               home
body_class:           home
title:                "Hi, I’m Editorial<br /> by HTML5 UP & Middle Bear"
subtitle:             My overridden site.tagline
description:          "Check out the Github repo for the Editorial theme, or take a look at the code for this demo site, <a href='https://github.com/jekyll-theme-editorial/jekyll-theme-editorial.github.io/'>jekyll-theme-editorial.github.io</a>."
banner:
  url:                "https://github.com/middlebear/jekyll-theme-editorial"
  link_title:         "Visit the Editorial theme Github repo"
  button_text:        "Github Repo"
images:
  banner:
    file:             "pic10.jpg"
    alt_text:         "Photo of a woman's torso holding a book and wearing a sleeveless top showing the tatoos along her right arm."
    title:            "photo: Annie Spratt, https://unsplash.com/photos/DYROsn8AyDI/"
# NOTE: features are set in `/_data/features.yml`
---

<!-- Banner -->
{%-include responsive_banner.html-%}

<!-- Section - Features -->
{%-include features.html section_title="Cool Features"-%}

<!-- Section - Articles -->
{%-include articles.html section_title="Neat Articles"-%}