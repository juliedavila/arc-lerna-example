# Example of an arc repo with Lerna enabled

## DIY setup

1. install architect`npm install @architect/architect`
1. install lerna `npm install lerna --save-dev`
1. init lerna `npx lerna init`
1. modify `lerna.json` so that the `packages` property contains at least `"src/http/*"`, but feel free to include any other directories that arc subject to the arc hydrate workflow.
1. go into each one of your sub directories in `src` and run `npm init --yes` if they have not already been initialized
1. profit

## New powers

1. Install a dev dependency into all of your arc functions: `npx lerna add standard --dev`
1. List all of your arc functions `npx lerna list`
1. Test your functions (think unit-level) `npx lerna run test`