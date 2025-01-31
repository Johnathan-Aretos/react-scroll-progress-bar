# react-scroll-progress-bar

React Component for a fixed scroll progress bar. The progress bar can use the default color and height, or can be customized by any user provided height and color.

## Install

```npm
npm install react-scroll-progress-bar
```

## Usage

### Default Progress Bar:

```jsx
import React from "react";
import ProgressBar from "react-scroll-progress-bar"; //Add this line

export default class App extends React.Component {
    render() {
        return (
            <div>
                <ProgressBar />
                //This is all you need to get the default view working
            </div>
        );
    }
}
```

----

### Custom Progress Bar:

```jsx
import React from "react";
import ProgressBar from "react-scroll-progress-bar";

export default class App extends React.Component {
    render() {
        return (
            <div>
                <ProgressBar height="6" bgcolor="#000" duration="0.2" />
                  // Here you can add any react component or jsx
                  // Add ProgressBar at your top level component or Root component.
                  // Change height and background-color by setting respective props.
            </div>
        );
    }
}
```

----

### Configuration:

```javascript
    <ProgressBar
      height="3"
      bgcolor="#F43059"
      duration="1"
      top="0"
      zIndex="99"
    />
```

**height** -- Set height of progress bar. Default height is `3px`. Pass the number not the unit. Unit is `px`

**bgcolor** -- Set background-color of progress bar. Default background-color is `#F43059`.

**duration** -- Set timing-duration for transition property. Default is `1s`. Pass the number not the unit. Unit is `s`

**top** -- Set the top value. Default is `0`. Pass the number not the unit. Unit is `px`

**zIndex** -- Set the zIndex value. Default is `99`. Pass a number. 

----
