# Mendix-Camera-Widget
Use the native camera without the use of Phonegap

## Installation
1. Download and Install npm from here https://nodejs.org/en/download/
2. open up Command line or Powershell and type in `npm install --global gulp-cli`
3. Navigate to the Mendix-Camera-Widget folder in explorer and edit package.json
4. in package.json do 2 things:
- under scripts section, add in  `"preinstall": "npx npm-force-resolutions"` so it'll look something like this
```json
"scripts": {
    //Your current package.json scripts
    "preinstall": "npx npm-force-resolutions"
},
```
- add a new section 
```json
"resolutions": {
    "graceful-fs": "^4.2.4"
 }
```
5. Save package.json
6. Reopen Command line or Powershell
7. Navigate to the Mendix-Camera-Widget folder in the CLI and type `npm install` 
8. After npm install is finished, `gulp build`
9. You can find your compiled package in "dist" folder.
