# Foundation

## Loaning Objections
- List 3 ways Foundation is different from Bootstrap
- Describe a situation in which using Foundation might be preferable to using Bootstrap, and a situation in which the reverse is true
- Explain what is meant by "breadcrumbs"

## How's this different from Bootstrap?

Wow. We get *way* more changes out-of-the-box.

Plus, we get some extras, like Modernizr, Normalize, Fastclick, and some jQuery plug-ins.

#### What is Modernizr?

Foundation also gives us some more explicit instructions in their documentation:

- They want us to name our custom stylesheet `app.css`
- They want us to include a `meta viewport` tag
- They want us to include Noramlize

...and who am I to disagree?

## Take 5 minutes to check out the kitchen sink

http://foundation.zurb.com/docs/components/kitchen_sink.html

#### What are your impressions?

## Take another 5 minutes to look at examples of Foundation in the wild

http://foundation.zurb.com/learn/website-examples.html

#### What do you think?

[Kelly Clarkson uses Foundation](http://www.kellyclarkson.com/us/), so it must be good!

## Foundation is definitely a framework

It's significantly more explicit than Bootstrap. It has to be: it's all about mobile-first development, which requires a lot of juggling in order to suit all mobile browsers' needs.

There are some visual cues to this end: the colors are much more vibrant than were Bootstrap's, and there are fewer gradients. This is to make things stand out more on a smaller screen that is likely surrounded by distractions.

All in all, foundation gives you comparatively little flexibility: things *have* to be set up a certain way.

#### Why would anyone want to use such a rigid framework?

Because, a la 1984, there's freedom in obedience. Rails requires you to write code in a specific way, but as a result, it does a lot of things for you that you'd otherwise have to worry about. Ditto for Foundation.

## Foundation also basically requires Javascript

Much of the Foundation functionality has to be explicitly linked in. That is: you have to explicitly link to the script for sidebar menus.

In order to make this Javascript work, you **must** include in your main Javascript file:

```js
$(document).foundation();
```

...and that's it. Unfortunately, the placement of this matters. It has to be run *after* everything else has finished loaded. So it needs to go inside `$(document).ready`, or in between `<script>` tags right at the end of your HTML as the last thing before `</body>`.

## Like Bootstrap

...it's got 12 columns.

Also like Boostrap, it has a lot of goofy terms:

- Off-canvas
- Magellan
- Breadcrumbs
- Orbit Slider
- Clearing Lightbox
- Flex Video
- Joyride

#### Take 5 minutes with your table partner to figure out what these are.

Breadcrumbs aren't a Foundation-specific thing at all.

## Unlike Bootstrap

...Foundation is intended to get you up and running ASAP. For instance, it comes with a "Pricing Table" module:

http://foundation.zurb.com/docs/components/pricing_tables.html

It also ships with a very handy form validator called Abide:

http://foundation.zurb.com/docs/components/abide.html

#### True or false: If you validate a form on the front-end, you don't really need to validate the form on the back-end.

False. Javascript validation can only be relied upon to give people notifications that they entered something incorrectly. Bypassing your validators is as easy as using "inspect element".

## Foundationify Grumblr

Checkout `master` to get the original Grumblr, create a new branch, and try adding in Foundation!

https://github.com/ga-dc/grumblr_css_redesign