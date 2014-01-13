# validate.js 日本語版

validate.js is a lightweight JavaScript form validation library inspired by CodeIgniter.
validate.jsはCodeIgniterにインスパイアされて開発された検証ライブラリのJavaScript軽量フレームワークです。

## Features

- Validate form fields from over a dozen rules
- No dependencies
- Customizable Messages
- Supply your own validation callbacks for custom rules
- Chainable customization methods for ease of declaration
- Works in all major browsers, (even IE6!)
- Modeled off the CodeIgniter form validation API

## How to use

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

## Documentation

You can view everything at http://rickharrison.github.com/validate.js

## Plugins

jQuery: https://github.com/magizh/validate_helper

## Japanese-Language Support

Japanese - https://github.com/bossatama/validate.js
