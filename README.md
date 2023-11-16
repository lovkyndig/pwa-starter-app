# PWA Starter App
I'm using this repo to start building all my apps. You can do it, you to, if you want!

## Why use this starter?
I'm using it as a starter kit, because I want the same theme in all my apps, and fokus on the `content` when I'm writing _articles_.

Maybe the most important thing is that the `content` on my pages is heavy (and serious) - and its about words, not pictures or videos. 

When it takes about on hour to read only one article, you need the futrues in this repo with search-functionalities and collapseble accordions, and a amazing catalog with overview of the content.[^1]

## Setup Environment

1. clone this template, or download this project to your PC

2. run the command in terminal to install dependent packages

```bash
npm install
# OR
yarn install
```

:bulb: you should install [Node.js](https://nodejs.org/) first, and add the [yarn](https://yarnpkg.com/) (a package manager) globally in your local PC.

## Write Articles

run the command in terminal to start a development server

```bash
npn run dev
# OR
yarn dev
```

Wait a seconds you will see some output in the terminal, like `Local: https://localhost:3000` Then you can visit this url at your browser to preview the web page.

You can start to write some articles by creating some markdown files inside the :file_folder: `/content/article` folder.

:sparkles: Learn it by study the example article [here](https://github.com/Benbinbin/BlogiNote/blob/main/content/article/example/1.example-article-en.md).

## Deploy

1. run the command in terminal to pre-render the website[^2], AND for creating the pagefind-bundle.

```bash
yarn generate
```

2. You will get the `dist/` directory (symlink to `.output/public`), then you can deploy this folder to any static hosting server.

:bulb: Recommend to [deploy the project to Vercel](https://vercel.com/docs/deployments/git/vercel-for-github). If you want to deploy to other platform, please check out the [documentation of Nuxt](https://nuxt.com/docs/getting-started/deployment#static-hosting).

_Updated 02.11.2023_

[^1]: The content in the `article`-folder is a copy of the articles in the template that is used: [Create Google App](https://github.com/lovkyndig/create-google-app). This `template` can be used (instead of this starter-kit) if you are an _open-source-programmer_.
[^2]: I'm using generate to check if the website still is working, after big shanges in the code (if I'm unsure about the result). But also to generate a new pagefind-bundle (in _public_-folder), after big changes in the content.
