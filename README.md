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

```py
import moment
from datetime import datetime

moment.date("12-18-2012")

moment.date("12-18-2012", "%m-%d-%Y")
moment.date("2012-12-18")
moment.date("December 18, 2012")
moment.date("2 weeks ago")
moment.date("2 weeks from now")
moment.now()
moment.utcnow()
moment.utc("2012-12-18")
moment.unix(1355875153626)
moment.unix(1355875173626, utc=True)
moment.date(2012, 12, 18).date
moment.utc(2012, 12, 18).date
moment.now().format("YYYY-M-D")
moment.date(2012, 12, 18).strftime("%Y-%m-%d")
moment.date(datetime(2012, 12, 18)).timezone("US/Eastern").date
moment.date(datetime(2012, 12, 18)).locale("US/Central").date
moment.now().locale("US/Pacific").timezone("US/Eastern")
moment.utcnow().timezone("US/Pacific")
now = moment.utcnow().timezone("US/Pacific")
future = now.clone().add(weeks=2)

moment.date(2012, 12, 18).add(days=2).subtract(weeks=3).date
moment.utcnow().add(years=3, months=2).format("YYYY-MM-D h:m A")
moment.date(2012, 12, 19).add(hours=1, minutes=2, seconds=3)
moment.date(2012, 12, 19, 1, 2, 3).subtract(hours=1, minutes=2, seconds=3)
moment.now().replace(hours=5, minutes=15, seconds=0).epoch()
moment.now().replace(hours=5, minutes=15, seconds=0).epoch(rounding=False)
moment.now().replace(years=1984, months=1, days=1, hours=0, minutes=0, seconds=0)
moment.utc(2012, 12, 19).year == 2012
moment.now().seconds
moment.date("2012, 12, 19").replace(weekday=1).strftime("%Y-%m-%d")
moment.date(2012, 12, 19).replace(weekday=7).date
moment.date(2012, 12, 19).replace(weekday=-7).format("YYYY-MM-DD")
moment.utcnow().weekday
moment.utcnow().zero
```

