# Valo-Trade Mobile Application

This is the mobile version of the Valo-Trade application, developed using the Flutter framework.

## Introduction

The Valo-Trade mobile application extends the functionality of the Valo-Trade web application, providing users with an e-commerce platform to trade Valorant in-game items.

## Changelog Tugas 7
### Implementation Steps

1. **Creating a New Flutter Project with E-Commerce Theme.** Initialized a new Flutter project named `valo_trade_mobile`. Set up the project with the necessary dependencies and folder structure.

2. **Developing Three Simple Buttons with Icons and Text.** Created three buttons (`Lihat Daftar Produk`, `Tambah Produk`, and `Logout`) using `ItemHomepage` class that take the parameter Icon and Color. Used `GridView.count` to arrange the buttons in a grid layout.

3. **Implementing Different Colors for Each Button.** Assigned different shades of red to each button to distinguish them visually. Ensured consistent theming throughout the app.

4. **Displaying Snackbars with Specific Messages.** Used `InkWell` and `onTap` callbacks to detect button presses. Displayed a `SnackBar` with a message corresponding to the button pressed saying "Kamu telah menekan tombol {buttonName}":

### FAQ

1. **Explain what is meant by a stateless widget and a stateful widget, and explain the difference between them.**

    * **Stateless Widget**: A widget that does not change during the application's runtime. Stateless widgets do not hold an internal state that can change. Examples include the `Text`, `Icon`, and `Container` widgets, which only display static information.

    * **Stateful Widget**: A widget that can change during the application's runtime. Stateful widgets have an internal state that can change and trigger a UI update when the state changes. Examples include `Checkbox`, `Slider`, and `TextField` widgets.

    * **Differences**:
        - **State Management**: Stateless widgets do not have a mutable state, whereas stateful widgets have a mutable state that can change during runtime.
        - **Lifecycle Methods**: Stateful widgets have lifecycle methods like `initState()`, `setState()`, and `dispose()`, while stateless widgets do not.
        - **Use Cases**: Stateless widgets are used for static UI elements, while stateful widgets are used for interactive and dynamic UI elements.

2. **List the widgets you used in this project and explain their functions.**
    * **MaterialApp**: The root widget that applies material design to the application.
    * **Scaffold**: Provides the basic structure for a page, including the AppBar and body.
    * **AppBar**: Displays a bar at the top of the app with a title.
    * **Text**: Displays text on the screen.
    * **Icon**: Displays an icon.
    * **GridView.count**: Organizes widgets in a grid with a specified number of columns.
    * **Card**: Displays information in a card with elevation.
    * **InkWell**: Handles touch interactions on a widget and provides a visual effect.
    * **SnackBar**: Displays a brief message at the bottom of the screen.
    * **Column**: Arranges widgets vertically.
    * **Row**: Arranges widgets horizontally.
    * **Container**: A versatile widget for layout, styling, and sizing.
    * **Padding**: Adds space around a widget.

3. **What is the function of `setState()`? Explain which variables can be affected by this function.**
    * **Function of `setState()`**: Used in stateful widgets to inform the framework that there is a change in the internal state that requires a UI update. When `setState()` is called, Flutter reruns the `build()` method to re-render the UI with the updated state.

    * **Affected Variables**: All variables declared in the state class (e.g., `_MyHomePageState`) and used in the `build()` method. These variables are part of the widget’s internal state and can change during runtime.

4. **Explain the difference between `const` and `final`.**
    * The `const` and `final` keywords in Dart are both used to define immutable values, but they differ in when and how these values are assigned. A `const` variable is a compile-time constant, meaning its value is fixed and cannot change once assigned. It must be initialized at the time of declaration, and the value cannot depend on any runtime computation. For example, `const double pi = 3.14;` defines a constant `pi` that will always hold the value 3.14 and does not change throughout the program.

    * On the other hand, `final` is more flexible, as it allows a variable to be assigned at runtime. Once a final variable is assigned, its value cannot be modified, but it doesn’t require an immediate value at the time of declaration. A final variable can thus hold values that are only known at runtime, like the current date and time. For instance, `final DateTime now = DateTime.now();` sets the variable `now` to the current date and time at runtime, which then remains constant. In short, `const` is a compile-time constant and more restrictive, while `final` allows for runtime assignment, making it suitable for values known only during execution.


## Additional Information
[In progress]

## Contributing

Pull requests are welcome. For major changes or bug reports, especially from `asdos` or `friends`, please open an issue first to discuss what you would like to change. Cheers - Kukuh