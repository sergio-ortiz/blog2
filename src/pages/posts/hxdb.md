---
layout: "../../layouts/PostLayout.astro"
---
# Hot Crossed Buns 

### Hot
- Hono
- api endpoints
- micro web frameworks
- least minimal web frameworks
- maybe standard library is enough


### X'
- HATEOAS
- SSR, View transitions api + prefetching
- htmz
- htmx for reactive UIs written in html "no js" ~4kb cdn link
- hyperscript + htmx
- htmx + alpine.js
- jQuery 4?


### D

- DaisyUI because it brings bootstrap like component classes on top of tailwind which brings back end devs the famialarity of working with bootstrap but instead of being limmited to custom sass and classes you have all the tweakability of tailwind


### Buns

- raw sql no ORM bloat and highly portable
- would prefer to use SQLite if possible do to its portability
- turso, serverless sqlite
- js because dominates edge computing via winterCG compatible js engine like the one in most browsers super light weight, Hono on top of bun looks like a good option because JSX is handled by default on bun nd you can use html in hono automatically, its not a big bloated meta framework plus I get to use drizzle which is close enough to sql :P, and also bun comes with sqlite nd its on sqlite api so might not even need drizzle
---
Why bun? well first of all we need a runtime to take our javascript code and turn into instructions the computer can execute and, bun can do that faster than any tool known to man. it is also a module bundler, a blazingly fast package manager compatible w/ npm, and test runner for your javascript project. basically all you need to quickly develop server side projects in javascript. quick install of bun with an official shell command in seconds, run your javascript code faster than any other runtime, install node packages faster than any other package manager, testing is built in to test your code as any professional should. this is fine but the runtime has its own specially fast api's that significantly improve the dev experience out of the box without having to install any other packages. I can hash and verify a password hash with a simple method call on the bun class. I can start  an http server with Bun.serve which takes in object defining a port and fetch request function that returnse a respose object. execute sql to sqlite databases with the query method on an instance of the Database class which takes in a database. fortunatly bun comes with an sqlite database baked in. the bun serve can serve text/html and bun automatically handles jsx so u can make composeable html templates with an embedded data from sqlite. u get SQL, database, http server, composeable html templates all included sppeding up and simplifying development. maybe one day I will be forced to use typescript, well bun handles that automatically too.

I want an express like framework ontop of bun, hono works well with bun is 10x faster than express and even simpler api. it also handles jsx, html, and middleware for auth and cookies paired with bun hash can make auth a breeze. while alsohaving testing and other helpers like logging and dev methods to streamline development.

Goodby node express, hello bun and hono.
React sucks to use, htmx forget about dealing with js dom manipulation and ajax.
goodbye css, sass, and bootstrap. hello tailwind and DaisyUI.

Lets start at the beginning, the 90s: html, css, js. These are non-negotiables in web dev. html for the structure and content type and data, css for the styling and, js for interactivity. Someone wanted a personal homepage for each user made possible by a database containing user data to then be embedded in the html markup and then built to a web page and sent to the user, introducing php PersonalHomePage language. We then had various versions of this with different languages. 2007 we introduced a library jQuery to abstract common ux dom manipulations and ajax to simple class methods. 2011 we saw bootstrap abstracting common ui component styles to classes like btn for buttons. At this point the web stack looked like PHP for the html, Bootstrap for the css, jQuery for the javascript, along with a database MySQL. MERN = html, materialUI = CSS, React libraries = js. Next.js + Prisma = hml, tailwind = css, js = react. bun + hono = html, Tailwind + DaisyUI = css, htmx = js.

1. html, css, js: web page
2. php, bootstrap, jQuery, MySQL: web apps
3. node, express, Mongo, React: spa
4. Next.js, prisma, tailwind: meta frameworks
5. bun, hono, htmx, DaisyUI: hateoas


