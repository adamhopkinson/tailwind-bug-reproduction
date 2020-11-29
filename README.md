# TailwindCss v2 bug reproduction

Following the [Laravel-specific installation guide](https://tailwindcss.com/docs/guides/laravel), installation of Tailwind fails at the `npx tailwindcss init` stage.

## Steps to reproduce.

1. Clone this repo
2. `npm install`
3. `npx tailwindcss init`

At this stage, I'm getting:

```
npx: installed 84 in 5.511s
Cannot find module 'autoprefixer'
Require stack:
- /Users/adam/.npm/_npx/16279/lib/node_modules/tailwindcss/lib/cli/commands/build.js
- /Users/adam/.npm/_npx/16279/lib/node_modules/tailwindcss/lib/cli/commands/index.js
- /Users/adam/.npm/_npx/16279/lib/node_modules/tailwindcss/lib/cli/main.js
- /Users/adam/.npm/_npx/16279/lib/node_modules/tailwindcss/lib/cli.js
```  

See [Github issue #2936](https://github.com/tailwindlabs/tailwindcss/issues/2936) for details & discussion. 
