# Express-TS-Webpack-config
Express, TypeScript, Webpackを使う時の基本的な設定ファイル.  
参考文献はこちら
- https://qiita.com/IgnorantCoder/items/c9b79dbab8c1a34b769f

## 5つの設定ファイルを使うときは,
- `$ npm install --save express`
- `$ npm install --save-dev @types/express`
- `$ npm install --save-dev typescript ts-loader tslint tslint-loader tslint-config-airbnb`
- `$ npm install --save-dev webpack webpack-cli`  
をインストール.

## プログラムを作成した後は,
開発環境では,
- `$ webpack --config webpack.config.dev.js`
- `$ node dist/server.js`  
を実行.  
  
本番環境では,
- `$ webpack --config webpack.config.prob.js`
- `$ node dist/server.js`  
を実行.
