*This repository is a mirror of the [component](http://component.io) module [matthewmueller/throttle](http://github.com/matthewmueller/throttle). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/matthewmueller-throttle`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# throttle

  Underscore's [throttle](http://underscorejs.org/#throttle) as a component.

  Useful for rate-limiting events that occur faster than you can keep up with.

## Installation

    $ component install matthewmueller/throttle

## Example

```js
var throttle = require('throttle');

window.onscroll = throttle(scroll, 100);

function scroll() {
  console.log('y', window.scrollY);
}
```

## API

### throttle(fn, wait)

  Creates and returns a new, throttled version of the passed function, that, when invoked repeatedly, will only actually call the original function at most once per every wait milliseconds.

## License

  MIT
