# 📖 Widgetbook Setup Script  

[![License](https://img.shields.io/github/license/GianMen91/widgetbook_setup_script)](https://github.com/GianMen91/widgetbook_setup_script/blob/master/LICENSE)
[![Version](https://img.shields.io/github/v/release/GianMen91/widgetbook_setup_script)](https://github.com/GianMen91/widgetbook_setup_script/releases)
[![Last Commit](https://img.shields.io/github/last-commit/GianMen91/widgetbook_setup_script)](https://github.com/GianMen91/widgetbook_setup_script/commits)

## Overview  
This script automates the integration of [Widgetbook](https://widgetbook.io/) into your Flutter project. It scans your `lib` directory for all widgets (`StatelessWidget` and `StatefulWidget`) and generates corresponding Widgetbook use-cases, allowing you to preview them interactively.  

## Features  
- ✅ Automates the setup of a Widgetbook project within a 'widgetbook' directory, streamlining the steps outlined in the Widgetbook [Quick Start Guide](https://docs.widgetbook.io/guides/quick-start).
- ✅ Scans your Flutter project's `lib` directory for all widgets.  
- ✅ Generates use-cases for each widget and saves them in `widgetbook/lib`, preserving the original directory structure.  
- ✅ Runs `build_runner` to generate the required `main.directories.g.dart` file.

## Usage  
1. Place the script in the root directory of your Flutter project (same level as `lib`, `pubspec.yaml`, etc.).  
2. Open a terminal in the project root.  
3. Run the script:

```sh
bash widgetbook_setup.sh
```

# Running Widgetbook
Once the script is finished and the setup is complete, navigate to the widgetbook directory and start Widgetbook:

 ```sh
 cd widgetbook  
 flutter run
 ```

# Buy me a coffee

<a href="https://www.buymeacoffee.com/giancarlo.mennillo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
