```bash
git clone git@github.com:brillout/preact-vite3
cd preact-vite3/
pnpm install
pnpm run prod
```

As single line:

```bash
git clone git@github.com:brillout/preact-vite3 && cd preact-vite3/ && pnpm install && pnpm run prod
```

Go to [http://localhost:3000](http://localhost:3000) and observe following error:

```
ReferenceError: require is not defined in ES module scope, you can use import instead
This file is being treated as an ES module because it has a '.js' file extension and '/home/romuuu/tmp/preact-client-routing/dist/server/package.json' contains "type": "module". To treat it as a CommonJS script, rename it to use the '.cjs' file extension.
    at file:///home/romuuu/tmp/preact-client-routing/dist/server/assets/chunk-e13215ee.js:1:9
    at ModuleJob.run (node:internal/modules/esm/module_job:198:25)
    at async Promise.all (index 0)
    at async ESMLoader.import (node:internal/modules/esm/loader:409:24)
    at async pageFile.loadFile (/home/romuuu/tmp/preact-client-routing/node_modules/.pnpm/vite-plugin-ssr@0.4.0-beta.34_vite@3.0.0-alpha.9/node_modules/vite-plugin-ssr/dist/cjs/shared/getPageFiles/parseGlobResults.js:25:40)
    at async Promise.all (index 1)
    at async loadPageFilesServerSide (/home/romuuu/tmp/preact-client-routing/node_modules/.pnpm/vite-plugin-ssr@0.4.0-beta.34_vite@3.0.0-alpha.9/node_modules/vite-plugin-ssr/dist/cjs/shared/getPageFiles/analyzePageServerSide/loadPageFilesServerSide.js:8:5)
    at async Promise.all (index 0)
    at async loadPageFilesServer (/home/romuuu/tmp/preact-client-routing/node_modules/.pnpm/vite-plugin-ssr@0.4.0-beta.34_vite@3.0.0-alpha.9/node_modules/vite-plugin-ssr/dist/cjs/node/renderPage.js:373:69)
    at async renderPage_ (/home/romuuu/tmp/preact-client-routing/node_modules/.pnpm/vite-plugin-ssr@0.4.0-beta.34_vite@3.0.0-alpha.9/node_modules/vite-plugin-ssr/dist/cjs/node/renderPage.js:87:23)
```
