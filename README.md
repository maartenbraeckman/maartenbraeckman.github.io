# maartenbraeckman.github.io

My personal website, built with [Astro](https://astro.build) and lots of stickers. 🦊

Live at **https://maartenbraeckman.github.io**

## Run it on your computer

You need [Node.js](https://nodejs.org) 24 (or at least 22.23.4).

```sh
npm install      # once, to download Astro
npm run dev      # start a local server at http://localhost:4321 that refreshes as you edit
npm run build    # build the final site into dist/
npm run preview  # look at the built site before publishing
```

## Where things live

| What you want to change         | File                                    |
| ------------------------------- | --------------------------------------- |
| The "Now" section on the home page | `src/data/now.ts`                    |
| Add a project card              | new `.md` file in `src/content/projects/` |
| Write a blog post               | new `.md` file in `src/content/blog/`   |
| About / Contact text            | `src/pages/about.astro`, `src/pages/contact.astro` |
| Colors and shared styles        | `src/styles/global.css`                 |
| The menu at the top             | `src/components/Header.astro`           |
| The big animated name           | `src/components/Hero.astro`             |
| The light-switch cord           | `src/components/ThemeSwitch.astro`      |
| Images and files used as-is     | `public/`                               |

Every page in `src/pages/` becomes a URL: `about.astro` is `/about/`, `blog/index.astro` is `/blog/`.

## Old exercise

My first hand-written page still lives at [/oefening02/](https://maartenbraeckman.github.io/oefening02/) (files in `public/oefening02/`).

## Publishing

Every push to `main` builds the site and publishes it to GitHub Pages
(see `.github/workflows/deploy.yml`). In the repo's **Settings → Pages**, "Source" must be set to **GitHub Actions**.
