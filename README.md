# startup_namer

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.

## Creating Hello world

* This example creates a Material app. [Material](https://material.io/design/) is a visual design language that is standard on mobile and the web. Flutter offers a rich set of Material widgets.
* The main() method uses arrow (=>) notation. Use arrow notation for one-line functions or methods.
* The app extends StatelessWidget which makes the app itself a widget. In Flutter, almost everything is a widget, including alignment, padding, and layout.
* The Scaffold widget, from the Material library, provides a default app bar, title, and a body property that holds the widget tree for the home screen. The widget subtree can be quite complex.
* A widget’s main job is to provide a build() method that describes how to display the widget in terms of other, lower level widgets.
* The body for this example consists of a Center widget containing a Text child widget. The Center widget aligns its widget subtree to the center of the screen.

## Stateful widgets 

Stateless widgets are immutable, meaning that their properties can’t change—all values are final.

Stateful widgets maintain state that might change during the lifetime of the widget. Implementing a stateful widget requires at least two classes: 1) a StatefulWidget class that creates an instance of 2) a State class. The StatefulWidget class is, itself, immutable, but the State class persists over the lifetime of the widget.

## List Views

The ListView class provides a builder property, itemBuilder, that’s a factory builder and callback function specified as an anonymous function. Two parameters are passed to the function—the BuildContext, and the row iterator, i. The iterator begins at 0 and increments each time the function is called. It increments twice for every suggested word pairing: once for the ListTile, and once for the Divider. This model allows the suggested list to grow infinitely as the user scrolls.

- The itemBuilder callback is called once per suggested word pairing, and places each suggestion into a ListTile row. For even rows, the function adds a ListTile row for the word pairing. For odd rows, the function adds a Divider widget to visually separate the entries. Note that the divider may be difficult to see on smaller devices.
- Add a one-pixel-high divider widget before each row in the ListView.
- The expression i ~/ 2 divides i by 2 and returns an integer result. For example: 1, 2, 3, 4, 5 becomes 0, 1, 1, 2, 2. This calculates the actual number of word pairings in the ListView, minus the divider widgets.
- If you’ve reached the end of the available word pairings, then generate 10 more and add them to the suggestions list.

## ontap function

When a tile has been tapped, the function calls setState() to notify the framework that state has changed.