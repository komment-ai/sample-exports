## Description

A directory containing Java classes for custom UI components used in the Sensable Android application.


## Component Overview

The components in this directory are designed to provide custom UI functionality for the application. The directory contains a single class, `FontFitTextView`, which is a custom `TextView` that can automatically adjust its font size to fit the available space.


## Usage

To use the `FontFitTextView` component, simply add it to your layout XML file:
```xml
<io.sensable.client.component.FontFitTextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Example text" />
```
You can then customize the appearance and behavior of the component using the standard `TextView` attributes and methods.


## Implementation

The `FontFitTextView` class extends the standard `TextView` class and overrides the `onMeasure` method to adjust the font size based on the available space. The implementation is straightforward and well-documented, making it easy to understand and modify if needed.



