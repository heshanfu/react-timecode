# ⏳ react-timecode

Simple React component for displaying a timecode, with various formatting options.

## Install

Via [npm](https://npmjs.com/package/react-timecode)

```sh
npm install --save react-timecode
```

Via [Yarn](https://yarn.fyi/react-timecode)

```sh
yarn add react-timecode
```

## How to use

The `Timecode` component is setup to be configurable as it needs to be, and hopefully
nothing more. Below are the `props` you can set on the component, along with a
simple example.

### Properties

* `element:String` - Element to render the timecode within. (Default: `span`)
* `format:String` - Specifies the format to display the timecode. (Default: `H:?m:ss`)
  * `HH:mm:ss.sss` - (Example: 00:01:23.876)
  * `H:mm:ss.sss` - (Example: 0:01:23.876)
  * `H:?mm:ss.sss` - (Example: 01:23.876)
  * `H:?m:ss.sss` - (Example: 1:23.876)
  * `HH:mm:ss` - (Example: 00:01:23)
  * `H:mm:ss` - (Example: 0:01:23)
  * `H:?mm:ss` - (Example: 01:23)
  * `H:mm` - (Example: 0:01)
  * `H:?m:ss` - (Example: 1:23 - _Default_)
* `time:Number` - Time in milliseconds to display the timecode for. (Default: `0`)

### Example

```js
import Timecode from 'react-timecode';

...

  render() {
    const {
      time,
    } = this.state;

    return (
      <Timecode time={time} />
    );
  }

...

```

## Pairs well with...

* [react-timer-wrapper](https://github.com/ryanhefner/react-timer-wrapper)

## License

[MIT](LICENSE) © [Ryan Hefner](https://www.ryanhefner.com)
