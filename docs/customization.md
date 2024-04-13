# Customization

Mi Create has a very modular theming system, allowing for custom but powerful themes to be created.

---

## Theme Components 

A theme consists of 3 things:

- Icons
- Stylesheet
- Color Schemes

## Icons

Icons use the Free Desktop icon theme specification (<https://specifications.freedesktop.org/icon-theme-spec/icon-theme-spec-latest.html>). View the default icon theme for an example.

## Stylesheets

Mi Create uses Qt. Stylesheets are one of the ways frames, buttons, etc are styled in the application.

Qt Style Sheets have similar syntax to CSS. If you already know CSS, theming Mi Create through stylesheets will be a breeze.

Style sheets operate on rules known as "style rules". Style rules are defined through a QWidget name (e.g QLineEdit, QPushButton) and curly braces `{}`. Style rules can modify different attributes about the widget, background color, border, etc. 

For example:

```css
QGroupBox {
  background-color: palette(alternate-base);
  border: 1px solid palette(midlight);
  margin-top: 25px;
}
```

Where QGroupBox is the QWidget, background-color is the attribute and the value is set to a QPalette value "alternate-base".

You may read more on how stylesheets work at:

- <https://doc.qt.io/qt-6/stylesheet.html> 
- <https://doc.qt.io/qt-6/stylesheet-reference.html>

## Color Schemes

Color Schemes are defined by colorSchemes.json. The name of the scheme is a key and contained are 2 ColorGroups: 

- Base
- Disabled

In the respective ColorGroup, are a list of QPalette ColorRoles, listed at <https://doc.qt.io/qt-6/qpalette.html#ColorRole-enum>