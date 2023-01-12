# Astro Project Structure
Created : 📅2022-09-30 14:53

## Project Structure

Your new Astro project generated from the `create-astro` CLI wizard already includes some files and folders. Others, you will create yourself and add to Astro’s existing file structure.

Here’s how an Astro project is organized, and some files you will find in your new project.

### Directories and Files

[Section titled Directories and Files](https://docs.astro.build/en/core-concepts/project-structure/#directories-and-files)

Astro leverages an opinionated folder layout for your project. Every Astro project root should include the following directories and files:

-   `src/*` - Your project source code (components, pages, styles, etc.)
-   `public/*` - Your non-code, unprocessed assets (fonts, icons, etc.)
-   `package.json` - A project manifest.
-   `astro.config.mjs` - An Astro configuration file. (recommended)
-   `tsconfig.json` - A TypeScript configuration file. (recommended)

### Example Project Tree

[Section titled Example Project Tree](https://docs.astro.build/en/core-concepts/project-structure/#example-project-tree)

A common Astro project directory might look like this:

```
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   └-─ Button.jsx
│   ├── layouts/
│   │   └-─ PostLayout.astro
│   └── pages/
│   │   ├── posts/
│   │   │   ├── post1.md
│   │   │   ├── post2.md
│   │   │   └── post3.md
│   │   └── index.astro
│   └── styles/
│       └-─ global.css
├── public/
│   ├── robots.txt
│   ├── favicon.svg
│   └-─ social-image.png
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

### `src/`

[Section titled src/](https://docs.astro.build/en/core-concepts/project-structure/#src)

The `src/` folder is where most of your project source code lives. This includes:

-   [Pages](https://docs.astro.build/en/core-concepts/astro-pages/)
-   [Layouts](https://docs.astro.build/en/core-concepts/layouts/)
-   [Astro components](https://docs.astro.build/en/core-concepts/astro-components/)
-   [UI framework components (React, etc.)](https://docs.astro.build/en/core-concepts/framework-components/)
-   [Styles (CSS, Sass)](https://docs.astro.build/en/guides/styling/)
-   [Markdown](https://docs.astro.build/en/guides/markdown-content/)

Astro processes, optimizes, and bundles your `src/` files to create the final website that is shipped to the browser. Unlike the static `public/` directory, your `src/` files are built and handled for you by Astro.

Some files (like Astro components) are not even sent to the browser as written but are instead rendered to static HTML. Other files (like CSS) are sent to the browser but may be optimized or bundled with other CSS files for performance.

### `src/components`

[Section titled src/components](https://docs.astro.build/en/core-concepts/project-structure/#srccomponents)

**Components** are reusable units of code for your HTML pages. These could be [Astro components](https://docs.astro.build/en/core-concepts/astro-components/), or [UI framework components](https://docs.astro.build/en/core-concepts/framework-components/) like React or Vue. It is common to group and organize all of your project components together in this folder.

This is a common convention in Astro projects, but it is not required. Feel free to organize your components however you like!

### `src/layouts`

[Section titled src/layouts](https://docs.astro.build/en/core-concepts/project-structure/#srclayouts)

[Layouts](https://docs.astro.build/en/core-concepts/layouts/) are a special kind of component that wrap some content in a larger page layout. These are most often used by [Astro pages](https://docs.astro.build/en/core-concepts/astro-pages/) and [Markdown or MDX pages](https://docs.astro.build/en/guides/markdown-content/) to define the layout of the page.

Just like `src/components`, this directory is a common convention but not required.

### `src/pages`

[Section titled src/pages](https://docs.astro.build/en/core-concepts/project-structure/#srcpages)

[Pages](https://docs.astro.build/en/core-concepts/astro-pages/) are a special kind of component used to create new pages on your site. A page can be an Astro component, or a Markdown file that represents some page of content for your site.

 CAUTION

`src/pages` is a **required** sub-directory in your Astro project. Without it, your site will have no pages or routes!

### `src/styles`

[Section titled src/styles](https://docs.astro.build/en/core-concepts/project-structure/#srcstyles)

It is a common convention to store your CSS or Sass files in a `src/styles` directory, but this is not required. As long as your styles live somewhere in the `src/` directory and are imported correctly, Astro will handle and optimize them.

### `public/`

[Section titled public/](https://docs.astro.build/en/core-concepts/project-structure/#public)

The `public/` directory is for files and assets that do not need to be processed during Astro’s build process. These files will be copied into the build folder untouched.

This behavior makes `public/` ideal for common assets like images and fonts, or special files such as `robots.txt` and `manifest.webmanifest`.

You can place CSS and JavaScript in your `public/` directory, but be aware that those files will not be bundled or optimized in your final build.

 TIP

As a general rule, any CSS or JavaScript that you write yourself should live in your `src/` directory.

### `package.json`

[Section titled package.json](https://docs.astro.build/en/core-concepts/project-structure/#packagejson)

This is a file used by JavaScript package managers to manage your dependencies. It also defines the scripts that are commonly used to run Astro (ex: `npm start`, `npm run build`).

There are [two kinds of dependencies](https://docs.npmjs.com/specifying-dependencies-and-devdependencies-in-a-package-json-file) you can specify in a `package.json`: `dependencies` and `devDependencies`. In most cases, these work the same: Astro needs all dependencies at build time, and your package manager will install both. We recommend putting all of your dependencies in `dependencies` to start, and only use `devDependencies` if you find a specific need to do so.

For help creating a new `package.json` file for your project, check out the [manual setup](https://docs.astro.build/en/install/manual/) instructions.

### `astro.config.mjs`

[Section titled astro.config.mjs](https://docs.astro.build/en/core-concepts/project-structure/#astroconfigmjs)

This file is generated in every starter template and includes configuration options for your Astro project. Here you can specify integrations to use, build options, server options, and more.

See the [Configuring Astro Guide](https://docs.astro.build/en/guides/configuring-astro/) for details on setting configurations.

### `tsconfig.json`

[Section titled tsconfig.json](https://docs.astro.build/en/core-concepts/project-structure/#tsconfigjson)

This file is generated in every starter template and includes TypeScript configuration options for your Astro project. Some features (like npm package imports) aren’t fully supported in the editor without a `tsconfig.json` file.

See the [TypeScript Guide](https://docs.astro.build/en/guides/typescript/) for details on setting configurations.


## References
1. [Project Structure](https://docs.astro.build/en/core-concepts/project-structure/)

## Advancements 