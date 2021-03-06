# React Native Persian SnackBar Component
A persian snackbar component for Android and iOS, customizable and simple.

![Snackbar demo](http://uupload.ir/files/enlh_screenshot_2017-12-26-00-32-52-864_com.testnavigation.png)


See [Google Material Design](https://material.io/guidelines/components/snackbars-toasts.html) for more info on Snackbars.

## Installation

```sh
npm install --save react-native-persian-snackbar-component
```

## Basic Usage

```javascript
import SnackBar from 'react-native-persian-snackbar-component'
```

## Code

```js
<SnackBar visible={true} textMessage="RTL Text" actionHandler={()=>{console.log("snackbar button clicked!")}} actionText="Lets go!"/>
```
## Options
| Prop        | Type           | Effect  | Default Value |
| ------------- |-------------| -----| -----|
| visible | boolean | Show or hide the snackbar | none |
| textMessage | string | The main message text | none |
| actionHandler | function | Function to be called when button is pressed, if absent no action button is shown | none |
| actionText | message | The text of action button, will be uppercased automatically | none |
| backgroundColor | color | The background color of snackbar | #484848 |
| accentColor | color | The color of action button text | orange |
| messageColor | color | The color of main message text | #FFFFFF |
| distanceCallback | function | Function to be caled whenever snackbar moves in and out or changes layout, the function will be supplied a number indicating distance taken up by snackbar on bottom. | (distance) => {} |
| bottom | number | The starting bottom position of snackbar | 0 |
| position | string | The position of the snackbar: top, bottom | bottom |

## Note

* When visible prop is changed, the snackbar will be animated in/out of screen
* The snackbar will not auto-dismiss by itself, for auto-dismiss use setTimeout() and change value passed to prop to false. 
* This works great together with [react-native-fab](https://github.com/SiDevesh/React-Native-FAB). See [demo](https://github.com/SiDevesh/snackbar-and-fab-demo) for example and instructions how to.

