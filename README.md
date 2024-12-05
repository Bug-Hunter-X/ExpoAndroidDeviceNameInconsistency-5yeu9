# Inconsistent Device Name Retrieval with Expo's Constants.deviceName API on Android

This repository demonstrates a bug in Expo's `Constants.deviceName` API where the returned device name on Android devices is inconsistent and may return an empty string or an unexpected value. This issue is more likely to occur on devices running custom ROMs or older Android versions.

## Bug Description
The `Constants.deviceName` API, intended to retrieve the device's name, fails to reliably provide the correct name on certain Android devices. The inconsistency of results makes it unsuitable for applications that depend on accurate device identification.

## Reproduction
1. Clone this repository.
2. Run the `bug.js` file using Expo Go or a similar Expo environment.
3. Observe the inconsistencies in the reported device name.

## Solution
The provided `bugSolution.js` demonstrates a more robust approach to get device name. It combines multiple methods to increase the chances of getting a valid device name.  Note that perfect reliability is still not guaranteed due to Android's inconsistencies across devices and versions.

## License
MIT