---
layout: "../../layouts/PostLayout.astro"
---


### I love Kanye, he's super crazy, I love his music. I am trying to compile my own personal donda. I dont care for his conspiracy theories.

---
I want to say that my application development architecture has gone and will probably continue to go something like this:

1. html, css, js + node + heroku + mongo
2. Next.js + prisma "heroku postgres" + css modules + netlify
3. php&mysql + Bootstrap&Sass + lamp
4. SvelteKit + vercel postgres "neon" + DaisyUI + vercel
5. Astro + PicoCSS + sqlite + drizzle + htmx
---
7. Go + Pico CSS + htmx + sqlite

---

now for web site development my stack is Astro for the web framework, markdown for the content, Tailwind CSS for the styling with DaisyUI for Bootstrap like component classes, Github + Netlify for the CI/CD. now for app state a little bit of js but I will stick to hypermedia as the engine of application state (HATEOS). I think I figured out the steps of migrating my Next Sites to Astro. might switch out DaisyUI for shadcn for maintainability and lack of abstraction.

1. Migrate Site from Next to Astro following astro doc's migration guide, make sure everything is where it supposed to be in the ui.
2. Deploy to Netlify, make sure everything is working "form submissions".
3. migrate in astro pages from css modules to style blocks and global css for markdown layouts
4. migrate the rest of the react components to astro unless u need that levely of declarative reactivity and state along with the respective css modules to style blocks
5. Migrate Content to markdown with specific rendering handled by layouts.
6. Migrate from style block to tailwind
