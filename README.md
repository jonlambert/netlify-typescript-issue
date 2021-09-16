# TypeScript / Netlify issue repro

Attempting to add a TypeScript function to an existing JavaScript project fails with the following:

```txt
Failed reloading function test with error:
Cannot destructure property 'inputs' of '(intermediate value)' as it is undefined.
```

Seems to be an issue with configuration. I've created this minimal reproduction including the `netlify.toml` file from the project in which I encountered the issue. Removing this file seems to fix the issue.

## To reproduce

Clone this repo, run:

```bash
npm install
netlify dev
```
