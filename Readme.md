# request-summary

    Return a request summary.

## Example

```js
var Summary = require('request-summary');

var app = express();
app.get(function (req, res, next) {
    var summary = Summary(req, res);
    console.log('Bytes received: ' + summary.requestSize);
    next();
});
```

## API

### .summary(req, res)
    
    Return an object summarizing a request.