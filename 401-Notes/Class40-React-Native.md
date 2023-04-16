# React Native

## getting started with react native

Name three Core Components of React Native and describe what they do.

1. <View>	<ViewGroup>	<UIView>	A non-scrolling <div>	A container that supports layout with flexbox, style, some touch handling, and accessibility controls.
2. <Text>	<TextView>	<UITextView>	<p>	Displays, styles, and nests strings of text and even handles touch events.
3. <Image>	<ImageView>	<UIImageView>	<img>	Displays different types of images.

What problem does React Native solve (why call it native)?

React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code. You can learn more about React in the next section. But first, let’s cover how components work in React Native.

In Android development, you write views in Kotlin or Java; in iOS development, you use Swift or Objective-C. With React Native, you can invoke these views with JavaScript using React components. At runtime, React Native creates the corresponding Android and iOS views for those components. Because React Native components are backed by the same views as Android and iOS, React Native apps look, feel, and perform like any other apps. We call these platform-backed components Native Components.

React Native comes with a set of essential, ready-to-use Native Components you can use to start building your app today. These are React Native's Core Components.

React Native also lets you build your own Native Components for Android and iOS to suit your app’s unique needs.

What are the building blocks of a React Native app? How does that compare to a React app?

Text and TextInput View 

## expo

What solution does expo provide?

Expo aims to provide a place where developers can create react native apps for mobile devices. Using expo you can develop, deploy, and debug.

Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.



What is the difference between React Native and Expo?

Expo flipped React Native development on its head by replacing how compilation, deployment, and testing worked. In particular, Expo features four major components: Expo—an open-source framework for building React Native apps with consolidated logic for both iOS and Android.

## expo snack

Checkout this tool. What does snack allow you to do?

Expo tries to manage as much of the complexity of building apps for you as we can, which is why we call it the managed workflow.

## ejecting

What does “eject” mean within the context of Expo?

The term "eject" was popularized by create-react-app, and it is used in Expo to describe leaving the cozy comfort of the standard Expo development environment, where you do not have to deal with build configuration or native code. When you "eject" from Expo, you have two choices:

Eject to bare workflow, where you jump between workflows and move into the bare workflow, where you can continue to use Expo APIs but have access and full control over your native Android and iOS projects.
Eject to ExpoKit, where you get the native projects along with ExpoKit. This option is deprecated and support for ExpoKit was removed after SDK 38.

When should you not eject?

Here are some situations where you may want to avoid ejecting from Expo:

If you are just starting out with mobile app development and are not yet comfortable with React Native or native development tools.

If you are working on a small or simple app that does not require advanced functionality or custom native modules.

If you are working with a tight deadline or limited resources, and need to get your app to market quickly without spending time on custom development.

If you want to take advantage of Expo's built-in features such as push notifications, analytics, and OTA updates, without having to set them up yourself.

Why might you choose to eject?

The Expo Eject Step is necessary to eject your app to install any missing native dependencies.


[link-to-reading-notes](https://facebook.github.io/react-native/docs/getting-started).
[link-to-reading-notes](https://expo.io/).
[link-to-reading-notes](https://snack.expo.io/).
[link-to-reading-notes](https://docs.expo.io/versions/latest/expokit/eject).
[link-to-reading-notes](https://facebook.github.io/react-native/docs/tutorial)
*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?