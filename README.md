[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FMeekLogic%2FWeight.js.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FMeekLogic%2FWeight.js?ref=badge_shield)

Weight.js
=========
JavaScript classes to convert imperial mass units as well as output and parse as text.

Install
-------
```javascript
npm install weight.js
```

Usage
-----
**ES6**
```javascript
import {Ounces, Pounds} from 'weight.js/src/weight';
//or
import Ounces from 'weight.js/src/ounces';
//or
import Pounds from 'weight.js/src/pounds';
```

**CommonJS**
```javascript
var Weight = require('../dist/weight.js');
var Ounces = Weight.Ounces;
var Pounds = Weight.Pounds;
//or
var Ounces = require('../dist/weight.js').Ounces;
//or
var Pounds = require('../dist/weight.js').Pounds;
```

Example
-------
```javascript
let ounces = Ounces.parse('5lbs  4 oz');

console.log(ounces.value); // 84

ounces.add(new Ounces(6));

console.log(ounces.value); // 90

if (ounces.isSame(new Ounces(90))) {
    console.log(ounces.toString()); // "5 lbs 10 oz"
}
```

Functions
---------
### Static
- **parse**

### Object
- **floor**
- **ceil**
- **round**
- **toFixed**
- **add**
- **subtract**
- **isSame**
- **isNotSame**
- **isHeavier**
- **isLighter**
- **isEmpty**
- **toString**
- **toOunces** (only for Pounds)
- **toPounds** (only for Ounces)


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FMeekLogic%2FWeight.js.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2FMeekLogic%2FWeight.js?ref=badge_large)