# Bare Bones ESLint & Code Formatting setup for Vue.js


#### Install package and dependencies 
```
npx install-peerdeps --dev eslint-config-tme-vue
```

#### Create and configure your .eslintrc
```
touch .eslintrc
```
Add the following to your .eslintrc
```json
{
	"extends": "tme-vue"
}
```

#### Add scripts to package.json
Add the following two script to your package.json file
```json
"scripts": {
	"lint": "eslint --ext .js,.vue src",
	"lint:fix": "eslint --ext .js,.vue src --fix"
},
```

#### Run lint

This command will simply display any errors or warnings your code may have

```
npm run lint
```

#### Run lint and attempt to fix errors

This command will attempt to fix any errors or warnings that don't follow the rules

```
npm run lint:fix
```