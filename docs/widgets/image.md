# Image
The Image widget is the most basic widget. It displays bitmap images

---

## Detailed Description
The Image widget displays images provided in the Image property. Width and Height are automatically set by the image.

There are 2 RGB formats the image will use: RGB565 and RGBA32. These are selected through a postfix on the widget's name, either _RGB or _RGBA (e.g Image_RGBA).

RGB565 has no alpha channel meaning no transparency support but smaller file size while RGBA32 has transparency but has a larger file size. Its good practice especially on older watches with no watchface compression to use RGB rather than RGBA if the image does not require transparency.

---

## Properties
#### General

|Name `@Name`|
|:----------|
|Widget name|

#### Position

|X `@X`|
|:----------|
|Horizontal position|

|Y `@Y`|
|:----------|
|Vertical position|

|Width `@Width` (disabled)|
|:----------|
|Widget width, automatically set by image|

|Height `@Height` (disabled)|
|:----------|
|Widget height, automatically set by image|

#### Appearance

|Alpha `@Alpha`|
|:----------|
|Widget transparency|

|Visibility Trigger `@Visible_Src` (some watches)|
|:----------|
|Display the widget based on the source's value|

#### Image

|Image `@Bitmap`|
|:----------|
|The image to be displayed|

---
## General

### Name `@Name`
The name of the widget.

---
## Position

### X `@X`
The horizontal position of the widget.

### Y `@Y`
The vertical position of the widget.

### Width `@Width`

The width of the widget. This property is automatically set by the image's width.

### Height `@Height`

The height of the widget. This property is automatically set by the image's height.

---

## Appearance

### Alpha `@Alpha`
The alpha value (transparency) of the widget.

### Visibility Trigger `@Visible_Src`
Determines the widget's visibility based on a source's value. The widget is hidden when the value of the source is 0, otherwise it is visible. **This property is only visible on Xiaomi Watch Color/Color Sport/Color 2/S1/S1 Pro/S2**

---

## Image

### Image `@Bitmap`
The image to be displayed on the widget.


