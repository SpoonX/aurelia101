# Troubleshooting
Some tipps when running into problems.

## Check the skeleton-navigation app
* Usually it's not a good idea to use newer packages than the official [skeleton-navigation](https://github.com/aurelia/skeleton-navigation) app. Compare the `package.json` files and upgrade or downgrade accordingly.
* Compare the `./build` diretories. Other then the `export.js` and the `bundles.js`, all files should be the same. 
* Before export or bundle, make sure you have the `export.js` and the `bundles.js` updated according to your project.

## Rebuild your project
Rebuilding your project as follows can help. Currently, a local installation of jspm@0.16.15 (`npm install jspm@0.16.15 --save`) is advised.
* `npm prune`
* `npm install`
* delete the jspm_packages folder `rm -rf ./jspm_packages`
* delete the map entry in `config.js`
* `jspm install`
