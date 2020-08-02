---
layout:               home
body_class:           home
title:                "Hi, I’m Editorial<br /> by HTML5 UP & Middle Bear"
subtitle:             My overridden site.tagline
description:          "Aenean ornare velit lacus, ac varius enim ullamcorper eu. Proin aliquam facilisis ante interdum congue. Integer mollis, nisl amet convallis, porttitor magna ullamcorper, amet egestas mauris. Ut magna finibus nisi nec lacinia. Nam maximus erat id euismod egestas. Pellentesque sapien ac quam. Lorem ipsum dolor sit nullam."
banner:
  url:                "/about"
  link_title:         "Read About Editorial"
  button_text:        "Learn More"
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