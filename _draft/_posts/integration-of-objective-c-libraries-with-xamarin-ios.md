---
title: Integration of Objective-C libraries with Xamarin iOS
date: '2016-07-27 05:20:00'
categories:
- objective-c
- xamarin ios
- pinvoke
- cocoapods
summary: ''
layout: post
---
# Example

```objc
typedef NS_ENUM(NSInteger, SDStatusBarManagerBluetoothState)
{
  SDStatusBarManagerBluetoothHidden = 0,
  SDStatusBarManagerBluetoothVisibleDimmed,
  SDStatusBarManagerBluetoothVisibleConnected
};

@interface SDStatusBarManager : NSObject

@property (copy, nonatomic) NSString *carrierName;
@property (copy, nonatomic) NSString *timeString;
@property (assign, nonatomic, readonly) BOOL usingOverrides;
@property (assign, nonatomic) SDStatusBarManagerBluetoothState bluetoothState;

- (void)enableOverrides;
- (void)disableOverrides;

+ (SDStatusBarManager *)sharedInstance;
+
```

# ObjectiveC
 - Constructors in objective c is done via instance methods that follow a naming convention (`initWithString(xxxx`))
 - 

# Datatypes
Objective-C
.NET

* Objective-C is a dynamic lanaugage, with some type safety but the majority is untyped - arrays, dictionaries.

# Themes
* Adding C# type information to a dynamic language (Obj-C).
* Convert C _DEFINES_ into ENUMS.
* Translate Objective-C idioms into C# idoms.
* Rename Objective-C methods into methods that conform with the .NET framework design guidelines.

# Enums
* Exposed in Objective-C as constants, need converting to C# enum idoims.


# Enumerations and Structures

# Interface Definition



# Reading
* https://msdn.microsoft.com/en-us/library/ms229042(v=vs.110).aspx
* 
# Watching
* https://youtu.be/DV7cGR0ySgo