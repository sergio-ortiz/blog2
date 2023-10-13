---
layout: '../../layouts/BaseLayout.astro'
---
# The HERB Stack

### H
- htmx for reactive UIs written in html "no js" ~4kb cdn link

### E
- Edge functions if possible that can send html to the client
- if not plain serverless functions
- if not at least minimal web framework for APIs
- if it cant be helped full legacy backend architectures

### R
- raw sql no ORM bloat and highly portable
- would prefer to use SQLite if possible do to its portability

### B
- Bootstrap for quick and mock ups and full customization via Sass
- Established tool for quickly making pallatble styles for backend dev
- Industry standard for 10+ years
- Still recieves updates to the framework and support

This stack aims to simplify full stack web application dev making each part highly
portable and thereby very modular to suit your needs. For this reason the
non-negotiables are: htmx so that Backend dev is not wasted on fontend logic or
complicated builds because htmx is ~4kb via cdn,Bootstrap because its been the 
industry standard for designing UIs on the BackEnd for over 10+ years so its known 
there are alot of resources and history and it keeps iterating to make the life of 
backend devs easier by not having to worry about css and also alot of codebases are 
already running bootstrap in production, finally raw sql because its not that hard 
and its translatable from database to database and from back end to backend unlike 
ORM bloatware. the BackEnd is modular and can be quickly written in something like 
ruby w/ sinatra and then changed to suit your needs because they will ultimately 
all be doing the same thing: respond to http requsts with raw html and not json, 
execute database queries in raw sql, and interpolate those db values into the html.
