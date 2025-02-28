# ham-js - the library for all things ham radios

## Example

```typescript
  const usbDevice = ... // get webusb usbdevice from user
  const usbDriver = new CP2105Driver(usbDevice)
  const serialDriver = new SerialDriver(usbDriver)
  const ft891Driver = new FT891Driver(serialDriver)

  await ft891Driver.setVfo(14250000) // 🎉
```

## Overview

### 1. Interface ham radios and accessories from the browser or node

`ham-js/cat` and `ham-js/webusb-serial-drivers` allows you to build ...

### 2. Log your QSOs from anywhere

`ham-js/...` is a fully featured logging solution running entirely in the browser (including CAT control). It leverages IndexedDB and data sources such as Lotw and QRZ for saving QSOs.

### 3. Use digimodes straight from your browser

`ham-js/...` integrates several packages into a fully featured digimode suite which runs in the browser.

### 4. Experimental: Use speech recognition on your QSOs to streamline logging

`ham-js/...` helps you streamline your logging process by leveraging the speech synthesis API in your browser and pre-filling fields, such as callsigns and RST ratings.

### 5. WebAudio-based sound processing

`ham-js/...` contains several ways to enhance your audio using DSP algorithms implemented straight in the browser.

## Principles

* ✅ **`ham-js` is modular** - each package has a specific responsibility. For example cat commands can be constructed with `ham-js/cat` however this package does not perform any sending via serial ports. **This is to ensure packages of `ham-js` can be used in many contexts, like browsers, servers and embedded devices.**

* ✅ **`ham-js` is tested** - in order to maintain this project in the long-term automated testing is important. It also helps to define and explain interfaces for consumers to understand what the library does.

* ✅ **`ham-js` is documented** - in order for users to adopt the project into their own software they have to understand how to use it. We document ham-js at ...

## Packages

* `ham-js/cat` - vast library of CAT interfaces to ham radio devices, such as ham radios, antennas and amplifiers
* `ham-js/webusb-serial-drivers` - implements user-space drivers for common usb-to-serial chipsets so browsers can interface them without the need for installing drivers in the host system (meaning you can easily interface devices from phones without the need for building a native application)
* ...

## Contribution

We appreciate your contribution. Please refer to the individual package repositories for their specific rules regarding contribution.

Our general contribution guidelines are:
...

We use the special organisation repository `.github` for tracking the general development of the package (see [issue tracker](https://github.com/ham-js/.github/issues) there).

## Contributors

* Harm - fixed a typo ♥️

... github badges here
