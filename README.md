# FDND Component Library

Read more about creating a library [in the docs](https://svelte.dev/docs/kit/packaging).

Read more about storybook [in the storybook docs](https://storybook.js.org/docs).

We've installed two packages for testing, read up on [playwright for end-to-end testing](https://playwright.dev/docs/writing-tests) and [vitest for unit testing](https://vitest.dev/guide/learn/writing-tests.html).

## Showcase or preview app

Once you've installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

Everything inside `src/lib` is part of your library, everything inside `src/routes` can be used as a showcase or preview app and everything inside `src/stories` is part of storybook.

## Storybook

You can see all components in the project in a nicely formatted way using storybook, start it up using:

```sh
npm run storybook

```

## Building

To build your library:

```sh
npm pack

```

To create a production version of your showcase app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

To create a production version of storybook:

```sh
npm run build-storybook
```

## Publishing

Go into the `package.json` and give your package the desired name through the `"name"` option. Also consider adding a `"license"` field and point it to a `LICENSE` file which you can create from a template (one popular option is the [MIT license](https://opensource.org/license/mit/)).

To publish your library to [npm](https://www.npmjs.com):

```sh
npm publish
```
