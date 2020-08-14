# JetBrains
JetBrains Mono fonts for AOSP based build system

## Disclaimer
- All credits go to the [JetBrains](https://www.jetbrains.com/lp/mono) Team.

## Getting started
**1. Add this repository to your AOSP build root's `external/jetbrainsmono`**

**2. Import external/jetbrainsmono/fonts.mk**

This can be done by appending the following at some makefile in vendor repo:

`$(call inherit-product-if-exists, external/jetbrainsmono/fonts.mk)`

For the Android System to use the font families, you need to add the contents of [fonts-jetbrains.xml](fonts-jetbrains.xml) into a fonts_customization.xml

For instance, for my personal vendor repo, [see](https://github.com/GeoZac/android_vendor_unconv/blob/master/product.mk)

**3. Build Android**
