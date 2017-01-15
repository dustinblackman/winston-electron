# winston-electron

This is a slightly modified version of the [original winston console transport](https://github.com/winstonjs/winston/blob/master/lib/winston/transports/console.js) to work with [Electron](https://github.com/electron/electron).

## Install

```
npm i --save winston-electron
```

## Example

```javascript
import ElectronConsole from 'winston-electron';
import winston from 'winston';

const Log = new winston.Logger({
  transports: [
    new ElectronConsole({
      level: 'debug',
      handleExceptions: true
    })
  ]
});

````
