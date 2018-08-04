# react-countdown
A simple countdown timer component for React.js.

This package is inspired from the awesome [vuejs-countdown](https://github.com/hashemirafsan/vuejs-countdown) package.

![screenshot](https://raw.githubusercontent.com/hashemirafsan/react-countdown/master/scr.png "React Countdown")

## Installation
#### npm

`npm i react-countdown --save`


## Usage

```javascript
import React, { Component } from 'react';
import CountDown from 'react-countdown';

class Something extends Component {
    constructor(props) {
        // something
    }

    render() {
        return(
            <div>
                <CountDown
                    deadline="August 22, 2022"
                />
                or
                <CountDown
                    end="August 22, 2022"
                />
            </div>
        );
    }
}

export default Something;
```

## Other Config

You can stop the countdown timer anytime by passing `true` (Boolean) with `stop` props.


### Caution 

Please don't provide any confusing date format since it has no dependency to Moment.js or any other date helpers. You can check [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/parse#Examples){:target="_blank"} more date format.