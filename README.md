# Widgetbook Setup Script

## Overview
This script automates the integration of Widgetbook into your Flutter project by generating Widgetbook use-cases for all widgets in the project’s `lib` directory. It scans the source directory for widgets (both StatelessWidget and StatefulWidget), and for each widget it creates a corresponding use-case in the Widgetbook project.

## The script:
1. Sets up a Widgetbook project in a `widgetbook` directory.
2. Scans the source code in the `lib` directory of your app for all widgets.
3. For each widget, it generates a use-case that wraps the widget and allows it to be viewed in the Widgetbook.
4. All generated use-cases are saved in the `widgetbook/lib` directory, replicating the structure of the source project, and using the same widget class names.
 5. Finally, it runs `build_runner` to generate the necessary `main.directories.g.dart` file for the Widgetbook.

## To use this script:
1. Place it in the root directory of your Flutter project (same level as `lib`, `pubspec.yaml`, etc.).
2. Run the script from the root directory of the project by executing `bash widgetbook_setup.sh`.
