---
layout: "../../layouts/PostLayout.astro"
---
# Stack
im thinking for web apps: HATEOAS + Pico CSS but for websites, astro with tailwind "DaisyUI".
the truth is go seems like the right choice for web apps but I am a js guy so this is why I would choose ~~node~~ bun + ~~express~~ hono for back-end.
we could later refactor to go, this is the beauty of HATEOAS is that the backend can be anything as long as the frontend isnt js dev. We would probably be refactoring from node + express to bun + hono anyways.
cutting edge as a whole seems to be moving away from nosql and towards sqlite tho, the gov has recently embraced postgres for db.
what is funny is astro is incorporating libsql/turso's fork of sqlite, and react moving more towards server rendering which will go hand in hand with hateoas.
people swear by go + htmx as the way. but react is moving towards server rendering and bun handles jsx and typescript out of the box, so we can send zero js to the client. bun has an easy to use http server with an in memory sqlite database and driver. bun has an easy to use file api for other files like html and jsx components. it has built in testing so for tdd. it also features password hashing and verifying for easy auth. all of this while being faster than node.
I want an express like framework ontop of bun, hono works well with bun is 10x faster than express and even simpler api. it also handles jsx, html, and middleware for auth and cookies paired with bun hash and verify can make auth a breeze. while also having testing and other helpers like logging and dev methods to streamline development. it can also do serverside rendering and doesn't force typescript like elysia.

# HATEOAS
- SSR, View transitions api + prefetching
- htmz
- htmx for reactive UIs written in html "no js" ~4kb cdn link, replace react/svelte/angular/vue
- hyperscript + htmx
- htmx + alpine.js
- htmx is a replacement for jQuery 4?

### CSS
- For most apps PicoCSS seems to do the trick, I think tailwind is good for refactoring but for quick mock ups u might not need it.
- DaisyUI because it brings bootstrap like component classes on top of tailwind which brings back end devs the famialarity of working with bootstrap but instead of being limmited to custom sass and classes you have all the tweakability of tailwind

### Backend
- api endpoints
- micro web frameworks
- minimal web frameworks
- maybe standard library is enough
- raw sql no ORM bloat and highly portable
- would prefer to use SQLite if possible do to its portability
- turso, serverless sqlite/libsql

---

Lets start at the beginning, the 90s: html, css, js. These are non-negotiables in web dev. html for the structure and content type and data, css for the styling and, js for interactivity. Someone wanted a personal homepage for each user made possible by a database containing user data to then be embedded in the html markup and then built to a web page and sent to the user, introducing php PersonalHomePage language. We then had various versions of this with different languages. 2007 we introduced a library jQuery to abstract common ux dom manipulations and ajax to simple class methods. 2011 we saw bootstrap abstracting common ui component styles to classes like btn for buttons. At this point the web stack looked like PHP for the html, Bootstrap for the css, jQuery for the javascript, along with a database MySQL. MERN = html, materialUI = CSS, React libraries = js. Next.js + Prisma = hml, tailwind = css, js = react. bun + hono = html, Pico = css, hateoas = js. go > js.

1. html, css, js: web page
2. php, bootstrap, jQuery, MySQL: web apps
3. node, express, Mongo, React: spa
4. Next.js, prisma, tailwind: meta frameworks
7. Astro + DaisyUI: Jamstack
5. bun, hono, htmx, Pico CSS: hateoas
6. go + htmx: HATEOAS + go > js

- node: front-end dev in js and now back end dev in js.
- express: the godfather of minimal/micro web-frameworks/no bloat/no batteries included. api endpoints, request response
- react: declaritive ui dev/reactivity with html in js like syntax "jsx" components: for better or worse react and jsx are now the standard.
- React sucks to use, htmx forget about dealing with js dom manipulation and ajax.
- also react is moving towards SSR 
- Goodbye node express, hello bun and hono. both improve the dev experience plus performance compared to node and express, also better docs.
- goodbye css, sass, and bootstrap. hello tailwind and DaisyUI. tho theres Pico CSS customizable w/ sass.
