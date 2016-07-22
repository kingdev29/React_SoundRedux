# React_SoundRedux

This repo is stolen from the awesome [soundredux](https://soundredux.io/) project by @andrewngu , I've been using it instead of the official Soundcloud client for a week.


### What I've learned

* Having redux as the data layer, it takes no effort to switch the view layer from DOM to react-native
* Writing CSS with flexbox is easy than normal CSS
* Building a native module for react-native is simple and straightforward thanks to the effort and nice design from Facebook
* Soundcloud API is awesome

Currently only focused on Android development because I don't have an iOS device and it's only fun when your code running on your own device.

The code is still a mess with ES6 + ES5 code mixed together. And I haven't done import all the features from soundredux and some of the code is even not used yet.

### Development

1. `npm install`
2. Check [Android Setup](https://facebook.github.io/react-native/docs/android-setup.html#content)
3. `react-native run-android`

Feedback, issues, etc. are more than welcome!

### TODO

- [x] InfinteScroll to load more songs
- [x] To be able to switch genre
- [ ] Clean up code
- [x] A modal to display song detail like the official client
- [ ] iOS

### Notes:

To run it on a real device, bundle the jsfile into the apk by running:

* create an assets folder under `android/app/src/main`
* curl "http://localhost:8081/index.android.bundle?platform=android" -o "android/app/src/main/assets/index.android.bundle"

Thanks to my awesome colleague [@xeodou](https://github.com/xeodou) who build the native Android player [react-native-player](https://github.com/xeodou/react-native-player)module on top of ExoPlayer.
