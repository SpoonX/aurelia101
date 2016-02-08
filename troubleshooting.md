# Troubleshooting
Some guide when running into problems.

## Check the skeleton-navigation app
* Usually it's not a good idea to use newer packages then the official [skeleton-navigation](https://github.com/aurelia/skeleton-navigation) app. Compare the `package.json` files and upgrade or downgrade accordingly.
* Compare the `./build` diretories. Other than the `export.json` and the `bundles.json` all files most likely should be the same. Make sure you have the `export.json` and the `bundles.json` updated according to your project.

## Rebuild your project

Rebuilding your project as follows can help. Currently, a local installation of jspm@0.16.15 (`npm install jspm@0.16.15 --save`) is advised.
* `npm prune`
* `npm install`
* delete the jspm_packages folder `rm -rf ./jspm_packages`
* delete the map entry in `config.json`
* `jspm install`
