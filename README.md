# jadepress-plugin-qr

[![Build Status](https://travis-ci.org/jade-press/jadepress-plugin-qr.svg?branch=master)](https://travis-ci.org/jade-press/jadepress-plugin-qr)

jade-press plugin which add qrcode api `/qr?text={text}`

## use
```javascript
//in jade-press config.js
exports.setting = {
    //...
    plugins: {
        'jadepress-plugin-qr': '*'
    }
    //...
}
```

then install

```bash
gulp install
```

## test
```bash

#for mongodb driver ubuntu (optional)
#sudo apt-get install libkrb5-dev
#or visit https://github.com/mongodb/node-mongodb-native#troubleshooting for more

#for canvas ubuntu (optional)
#sudo apt-get install libcairo2-dev libjpeg8-dev libpango1.0-dev libgif-dev build-essential g++
#visit https://www.npmjs.com/package/canvas for more platform

#makesure your mongodb service is running

git clone https://github.com/jade-press/jadepress-plugin-qr.git
cd jadepress-plugin-qr
npm install node-gyp -g
npm install mocha -g
npm install bower -g
npm install
bower install
npm i jadepress-theme-pi
mkdir node_modules/jadepress-plugin-qr
cp -r plugins node_modules/jadepress-plugin-qr/

# if edit file, run "gulp watch"
npm run test

# if npm install failed
```

