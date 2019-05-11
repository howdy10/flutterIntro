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