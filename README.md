If you want to apply the workaround here are the steps :

•⁠  ⁠Add the required package:

```
yarn add @videosdk.live/react-sdk@v0.2.3
```

•⁠  ⁠Directory structure (for reference):

```
node_modules
 └── @videosdk.live
      ├── js-sdk
      │    └── videosdk.js
      ├── react-sdk
      │    └── dist
      └── react-native-sdk
           └── node_modules
                └── @videosdk.live
                     ├── js-sdk
                     │    └── videosdk.js
                     └── react-sdk
                          └── dist
```

•⁠  ⁠Replace the files/folders as follows:

Replace:
node_modules/@videosdk.live/js-sdk/videosdk.js
with:
node_modules/@videosdk.live/react-native-sdk/node_modules/@videosdk.live/js-sdk/videosdk.js
 Replace:
node_modules/@videosdk.live/react-sdk/dist
with:
node_modules/@videosdk.live/react-native-sdk/node_modules/@videosdk.live/react-sdk/dist
