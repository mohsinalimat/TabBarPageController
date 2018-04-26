# TabBarPageController

[![CI Status](https://img.shields.io/travis/conmulligan/TabBarPageController?style=flat)](https://travis-ci.org/conmulligan/TabBarPageController)
[![Version](https://img.shields.io/cocoapods/v/TabBarPageController?style=flat)](https://cocoapods.org/pods/TabBarPageController)
[![License](https://img.shields.io/cocoapods/l/TabBarPageController?style=flat)](https://cocoapods.org/pods/TabBarPageController)
[![Platform](https://img.shields.io/cocoapods/p/TabBarPageController?style=flat)](https://cocoapods.org/pods/TabBarPageController)

`TabBarPageController` is a container view controller that manages navigation between tabs of content. Each tab is managed by a child view controller embedded in a `UIPageViewController` instance, allowing users to navigate between tabs by selecting tab bar items or swiping left and right.

## Usage

Create a `TabBarPageController` instance and add view controllers to it:

```swift
    let tabBarController = TabBarPageController()
    tabBarController.add(viewController)
```

Show a specific view controller:

```swift
    tabBarController.show(viewController)
```

Although `TabBarPageController` is similar to `UITabBarController` it is not a drop-in replacement and has a number of important differences:

- `TabBarPageController` always hides the tab bar when a child navigation view controller pushes a new view controller. This is to avoid interfering with the navigation controller's back navigation gesture.
- This is a test

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

Requires iOS 9 or greater.

## Installation

`TabBarPageController` is available through [CocoaPods](https://cocoapods.org). To install it, simply add the following line to your Podfile:

```ruby
pod 'TabBarPageController'
```

You can also just copy the `TabBarPageController.swift` file into your project.

## Author

conmulligan, conmulligan@gmail.com

## License

`TabBarPageController` is available under the MIT license. See the LICENSE file for more info.
