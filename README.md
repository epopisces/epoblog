# Getting Started

If Node and its managers aren't already installed, follow [this guide](https://docs.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows)

The version of webpack included in Gridsome doesn't (yet) support the newer hashes required by the openssl version included in node 17.x.  Downgrade node.js (they can be installed side-by-side on the system, and nvm can select which is active--note they have separate module install bases, so any necessary modules may need to be reinstalled)
```powershell
# install & select node.js 16.14.2
nvm install 16.14.2 (w/LA)
nvm use 16.14.2 (w/LA)

# install gridsom, clone down liebling starter
npm install --global @gridsome/cli
gridsome create epoblog https://github.com/jammeryhq/gridsome-starter-liebling
cd epoblog
npm install
```

Testing
```powershell
gridsome develop
```
## Adding Mermaid Support
```powershell
npm install gridsome-plugin-remark-mermaid
```
Modify `grisome.config.js` according to the [plugin docs](https://next.gridsome.org/plugins/gridsome-plugin-remark-mermaid)

Continue developing

## Fixing vulns

## Build/Deploying