# Branch Demo App Issue with getLatestReferringParams on Android

## Description of the problem

It seems that if the `branch.subscribe` method is not called before calling `branch.getLatestReferringParams`, the value returned by the latter will always be null. The issue appears to exist only on Android — on iOS, there is no need to call the `subscribe` method for `getLatestReferringParams` to work properly.

## Start the demo

Install the dependencies:

```sh
npm i
bundle install
cd ios & bundle exec pod install
```

Start the app:

```sh
npm run android
#or
npm run ios
```

You can use this quick link to test the integration with branch :
`https://fhfyd.test-app.link/invitation-accept`
