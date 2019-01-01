# Express-TS-Webpack-config
Express, TypeScript, Webpackを使う時の基本的な設定ファイル.  
参考文献はこちら
- https://qiita.com/IgnorantCoder/items/c9b79dbab8c1a34b769f

## 5つの設定ファイルを使うときは,
### npmを使う場合は,
- `$ npm install --save express`
- `$ npm install --save-dev @types/express`
- `$ npm install --save-dev typescript ts-loader tslint tslint-loader tslint-config-airbnb`
- `$ npm install --save-dev webpack webpack-cli`
- `$ npm install --save-dev webpack-node-externals`  
をインストール.  
まとめると,
- `$ npm install --save-dev @types/express typescript ts-loader tslint tslint-loader tslint-config-airbnb webpack webpack-cli webpack-node-externals`

### yarnを使う場合は,
- `$ yarn add express`
- `$ yarn add --save @types/express typescript ts-loader tslint tslint-loader tslint-config-airbnb webpack webpack-cli webpack-node-externals`

## Webpackを使うには, WebpackのPATHを通しておく.
macでは, *~/.bashrc*か, *~/.bash_profile*に  
`export PATH=$PATH:./node_modules/.bin`  
を追加する.

## プログラムを作成した後は,
### 開発環境では,
- `$ webpack --config webpack.config.dev.js`
- `$ node dist/server.js`  
を実行.  

もしくは, *package.json*の`"scripts":{}`のところに,
- `"test": "webpack --config webpack.config.dev.js && node dist/server.js"`  
を追加.

### 本番環境では,
- `$ webpack --config webpack.config.prob.js`
- `$ node dist/server.js`  
を実行.  

もしくは, *package.json*の`"scripts":{}`のところに,
- `"start": "webpack --config webpack.config.prob.js && node dist/server.js"`  
を追加.
