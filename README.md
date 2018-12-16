### moment
---
.js
https://github.com/moment/moment

https://momentjs.com/

.py
https://github.com/zachwill/moment

```js
moment().format('MMMM Do YYYY, h:mm:ss a');

moment("20181217").fromNow();

moment().subtract(10, 'days').calendar();
moment().calendar();

moment.locale();
moment().format('LT');



var moment = require('moment');
moment().format();

requirejs.config({
  packages: [{
    name: 'moment',
    location: '[bower_components|node_modules]/moment'
    main: 'moment'
  }]
});

define(['moment'], function(moment){
  console.log(moment().format('LLLL'));
});
define(['moment', 'moment/locale/de'], function(moment){
  moment.locale('de');
  console.log(moment().format('LLLL'));
});
define(['moment/min/moment-width-locales'], funciton(moment){
  moemnt.locale('de');
  console.log(moment().format('LLLL'));
});
define(['require', 'moment'], function(rquire, moment){
  require(['moment/locale/de'], function(LocaleModule){
    console.log(moment().format('LLLL'));
    moment.locale('de');
    console.log(moment().format('LLLL'));
  })
});

require.config({
  config: {
    moment: {
      noGlobal: true
    }
  }
});

var moment = require('moment');
moment.format();
```

```sh
npm install moment --save
yarn add moment
Install-Package Moment.js
spm install moment --save
meteor add momentjs:moment
bower install --save

npm install moment 
bower install --save moment
Install-Package Moment.js
meteor add momentjs:moment
npm install moment
```


```
<script src="moment.js"></script>
<script>
  moment().format();
</script>
```

