# Testing out some interesting tools

[Snowpack](https://www.snowpack.dev/), [TypeScript](https://www.typescriptlang.org/), [Svelte](https://svelte.dev/), [pnpm](https://github.com/pnpm/pnpm).

Clone the project, `pnpm start`

## Things to note on the stuff I'm new to:
### Svelte
1) I couldn't figure out a nice way to have encapsulated styles without clogging up the svelte files, the method used for importing the styles in this project leaks into other files. Seems you need the styles in the file, seems kinda messy... 
1) Not a fan of the svelty specific logic, prefer reacts JSX as you can just write JavaScript.
1) Still a new project, error messages aren't too helpful.
1) very very fast

### Snowpack
1) everything just worked, and it's super performant... why not.

### pnpm
1) everything just worked, and it's super performant... why not.

---

# New Project

> ✨ Bootstrapped with Create Snowpack App (CSA).

## Available Scripts

### npm start

Runs the app in the development mode.
Open http://localhost:8080 to view it in the browser.

The page will reload if you make edits.
You will also see any lint errors in the console.

### npm test

Launches the test runner in the interactive watch mode.
See the section about running tests for more information.

### npm run build

Builds a static copy of your site to the `build/` folder.
Your app is ready to be deployed!

**For the best production performance:** Add a build bundler plugin like [@snowpack/plugin-webpack](https://github.com/snowpackjs/snowpack/tree/master/plugins/plugin-webpack) or [snowpack-plugin-rollup-bundle](https://github.com/ParamagicDev/snowpack-plugin-rollup-bundle) to your `snowpack.config.json` config file.

### Q: What about Eject?

No eject needed! Snowpack guarantees zero lock-in, and CSA strives for the same.
