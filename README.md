# ineffablevoyage.github.io

A website for the ineffable voyage zines

This Website use the svelte framework 


## Developing

Start by installing the dependencies
```sh
npm install
```

Don't forget to also download the static adaptater if it's not already done for the github pages build
```sh
npm i -D @sveltejs/adapter-static
```

Once that's done, start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

This step is not needed as the website is automatically deployed on github pages when changes are push to the main branches, but in case you want a local build app, it's how to do it.

```sh
npm run build
```
