---
title:            "Interdum aenean"
author:           petunia
date:             2020-01-01 08:01:02 -0800
last_modified_at: 
categories:       [jekyll, editorial]
tags:             []
series:           "build-a-blog"
images:
  default:
    file:         pic01.jpg
    alt_text:     "i'm some alt text for this image."
    caption:      "Woohoo! This photo has a caption! What a great caption! Too excited! Can't use enough exclamation points!"
    title:        "Within minutes, and to her real horror, Julia realized she was encapsulated by the title attribute of the default image of this post."
# NOTE that the first paaragraph below is the excerpt, if no excerpt is defined here in the front matter.
---


Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.

## Aenean eget sagittis
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla est quam, efficitur nec tincidunt ac, finibus in leo. Ut volutpat tellus vitae velit viverra ultrices. Quisque nec congue massa, ultrices sagittis est. Quisque gravida suscipit mattis. Quisque volutpat leo lectus, nec tincidunt tellus sagittis eget. Proin nec dictum nunc. Aliquam odio urna, ultricies congue ante eget, sagittis semper lorem. Suspendisse condimentum lobortis nisl accumsan lobortis. Donec quis lacus eu neque egestas fermentum. Donec viverra lectus ac tellus bibendum pretium. Fusce feugiat tincidunt turpis, id facilisis quam rhoncus sit amet. Aenean eget sagittis est. Etiam velit dolor, facilisis ac quam sit amet, egestas pretium nisl.

## Fusce ut ornare lacus
!["Frankly my dear, I don't give a damn!"]({{site.image_path}}pic02.jpg "Dear Scarlett, From Rhett"){:.image.right}
Nullam consequat enim ut lacinia dapibus. Duis vitae eros ex. Phasellus fringilla mauris turpis, maximus vehicula mi ornare vel. Fusce ut ornare lacus. Etiam mattis varius lectus a mattis. Fusce in dapibus odio. Nam ut lobortis dui, sed malesuada nulla. Mauris eleifend tristique dui et molestie. Nullam hendrerit lacinia diam tempus ornare. Cras in vulputate ex, nec tempor sem. Cras a tellus rhoncus purus suscipit pretium vitae at dui. Aliquam a aliquam mauris. Cras sodales sagittis tellus a efficitur. 

<div class="row">
  <div class="col-4 col-12-medium">
    <h3>Interdum sapien gravida</h3>
    <p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit.</p>
  </div>
  <div class="col-4 col-12-medium">
    <h3>Faucibus consequat lorem</h3>
    <p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit.</p>
  </div>
  <div class="col-4 col-12-medium">
    <h3>Accumsan montes viverra</h3>
    <p>Nunc lacinia ante nunc ac lobortis. Interdum adipiscing gravida odio porttitor sem non mi integer non faucibus ornare mi ut ante amet placerat aliquet. Volutpat eu sed ante lacinia sapien lorem accumsan varius montes viverra nibh in adipiscing blandit.</p>
  </div>
</div>

{% capture text %}
## Phasellus viverra
Ut consectetur molestie risus suscipit porttitor. Phasellus viverra ex nec varius interdum. Mauris nec justo id odio convallis condimentum. Nunc est tortor, dignissim id porttitor at, condimentum non mi. Sed id elementum purus, ut euismod neque. Phasellus vel rhoncus leo. Phasellus eget imperdiet tortor. Suspendisse feugiat neque vel pulvinar placerat. Etiam posuere fringilla lacus, id rutrum massa aliquam at.
{% endcapture %}
{{ text | markdownify }}
