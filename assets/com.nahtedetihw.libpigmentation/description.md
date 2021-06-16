# libpigmentation

** libpigmentation offers the ability to obtain colors from an image. **

* Join my Discord today to report any issues: https://discord.gg/64kVRNzKnF

# Usage

## Installation in Theos

### Installation

1. Download this repository
2. Put the `.dylib` into your `theos/lib` folder
3. Put the `libpigmentation.h` file into your `theos/include` folder

## Configuration
1. Add `TWEAKNAME_LIBRARIES = pigmentation` to your makefiles (only to your tweak makefile if you only use the helper functions)
2. Add `com.nahtedetihw.libpigmentation` to the `Depends` in your `control` file

```objc
@interface libpigmentation : NSObject
-(NSDictionary *)coloursForImage:(UIImage *)image forEdge:(int)edge;
- (BOOL)isColorTooDark:(UIColor *)color;
- (BOOL)isColorTooLight:(UIColor *)color;
- (UIColor *)lighterColorForColor:(UIColor *)color;
- (UIColor *)darkerColorForColor:(UIColor *)color;
@end
```

### Source Code
https://github.com/nahtedetihw/libpigmentation

### Follow

* [**ETHN**](https://twitter.com/ethanwhited) - follow me for more up to date info, or ask me anything.

* [**Email**](mailto:ethanwhited2208@gmail.com) - open to any questions or concerns.
