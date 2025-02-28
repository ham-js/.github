# ham-js - the library for all things ham radios

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

* ✅ `ham-js`

## Packages

* `ham-js/cat` - vast library of CAT interfaces to ham radio devices, such as ham radios, antennas and amplifiers
* `ham-js/webusb-serial-drivers` - implements user-space drivers for common usb-to-serial chipsets so browsers can interface them without the need for installing drivers in the host system (meaning you can easily interface devices from phones without the need for building a native application)
* ...
