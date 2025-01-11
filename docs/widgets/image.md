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

|Name |
|:----------|
|Widget name|

#### Position

|X |
|:----------|
|Horizontal position|

|Y |
|:----------|
|Vertical position|

|Width (disabled)|
|:----------|
|Widget width, automatically set by image|

|Height (disabled)|
|:----------|
|Widget height, automatically set by image|

#### Appearance

|Opacity |
|:----------|
|Widget transparency|

|Visibility Trigger|
|:----------|
|Display the widget based on the source's value|
|*Only visible on Xiaomi Watch Color/Sport/2/S1/S1 Pro/S2*| 

#### Image

|Image |
|:----------|
|The image to be displayed|