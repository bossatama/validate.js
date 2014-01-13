# validate.js 日本語版

validate.jsはCodeIgniterにインスパイアされて開発された検証ライブラリのJavaScript軽量フレームワークです。

## 特徴

- 12以上の検証ルールからフィールドを検証できる
- ライブラリ非依存
- エラーメッセージをカスタマイズできる
- 独自カスタマイズルールを検証時にコールバックできる
- 宣言を容易にするためのカスタマイズメソッドチェーンできる
- 主要なWebブラウザで動作する（IE6も!）
- CodeIgniterのフォーム検証APIからモデル化

## 使い方

    var validator = new FormValidator('example_form', [{
        name: 'req',
        display: 'required',
        rules: 'required'
    }, {
        name: 'alphanumeric',
        rules: 'alpha_numeric'
    }, {
        name: 'password',
        rules: 'required'
    }, {
        name: 'password_confirm',
        display: 'password confirmation',
        rules: 'required|matches[password]'
    }, {
        name: 'email',
        rules: 'valid_email'
    }, {
        name: 'minlength',
        display: 'min length',
        rules: 'min_length[8]'
    }], function(errors) {
        if (errors.length > 0) {
            // Show the errors
        }
    });

## ドキュメント

You can view everything at http://rickharrison.github.com/validate.js

## プラグイン

jQuery: https://github.com/magizh/validate_helper

## 日本語化サポート

Japanese - https://github.com/bossatama/validate.js
