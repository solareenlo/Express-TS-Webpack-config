# Express-TS-Webpack-config

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
