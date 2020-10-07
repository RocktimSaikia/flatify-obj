# flatify-obj ![build](https://travis-ci.com/RocktimSaikia/flatify-obj.svg?branch=master) ![license](https://img.shields.io/github/license/rocktimsaikia/flatify-obj)

> Flatten nested javascript objects into a single-depth object.

## Install
```bash
npm install flatify-obj
```

## Usage

 ```js
    const flatifyObject = require('flatify-obj');

    flatifyObject({foo: {bar: {unicorn: '🦄'}}})
    //=> { 'foo.bar.unicorn': '🦄' }

    flatifyObject({foo: {unicorn: '🦄'}, bar: 'unicorn'}, {onlyLeaves: true});
    //=> {unicorn: '🦄', bar: 'unicorn'}
 ```

## API

### flatifyObject(object, options?)

#### object

Type: `object`<br>
Object to flatten


#### options

##### onlyLeaves

Type: `boolean`<br>
Default: `false`

Removes the parent property and only returns the leaf nodes of the object


## Support

<a href="https://www.buymeacoffee.com/7BdaxfI"><img src="https://user-images.githubusercontent.com/33410545/91206759-48d5d180-e725-11ea-93b5-754d98c007af.png" height="60px"/></a>
