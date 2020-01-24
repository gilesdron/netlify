---
layout: post
title:  "How this site was created and my tool selections."
---

# Site Generator.

I chose Jekyll from [https://www.staticgen.com/](https://www.staticgen.com/){:target="_blank"} for this exercise as the markup reminded me of MediaWiki (something I used in a previous life).  

I selected the ‘Deploy to Netlify’ option however this threw an exception as reported on [https://community.netlify.com/t/connection-refused-exit-status-128/7197](https://community.netlify.com/t/connection-refused-exit-status-128/7197){:target="_blank"}.  

To resolve I located and cloned [https://github.com/netlify-templates/jekyll-base](https://github.com/netlify-templates/jekyll-base){:target="_blank"} into [https://github.com/gilesdron/netlify](https://github.com/gilesdron/netlify){:target="_blank"} and then imported manually via [https://app.netlify.com/start/repos/gilesdron%2Fnetlify](https://app.netlify.com/start/repos/gilesdron%2Fnetlify){:target="_blank"}. This proved to be a solid workaround.

# Modifications.

- Added the following to _config.yml to fix future dates on posts and to enable redirects function for /anything to redirect to google.

future: true

include: /_redirects 

# Tools.

I used Github desktop to manage the Git source and MS Code as the IDE to create/edit the config & markup files as both are responsive and play well together.

# Development Environment.

Ferdora 31 Workstation with latest Ruby, RubyGems, GCC and make.  

[Back to home page](https://practical-galileo-423fde.netlify.com/)
