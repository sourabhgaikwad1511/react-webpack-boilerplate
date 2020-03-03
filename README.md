React bootstap app:

cmds:

	- npm init
	- npm  i react react-dom
	- npm i --save-dev webpack webpack-dev-server webpack-cli
	- npm i --save-dev babel-core babel-loader babel-preset-env babel-preset-react html-webpack-plugin


for warning :
npm WARN babel-loader@8.0.6 requires a peer of @babel/core@^7.0.0 but none is installed. You must install peer dependencies yourself.
solution :

	- npm install --save-dev @babel/core @babel/preset-env @babel/preset-react

	- add script in package.json to run and build command:
		"scripts": {
  			  "start": "webpack-dev-server --mode development --open --hot",
 			   "build": "webpack --mode production"
			  }
