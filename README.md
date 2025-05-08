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

### Option 1

You can use curl to download and execute the script in one command:

```sh
curl -s https://raw.githubusercontent.com/GianMen91/widgetbook_setup_script/main/widgetbook_setup.sh | bash
```

- `curl -s` fetches the script silently.
- The `| bash` part pipes it directly into a new Bash process.

### Option 2
1. Place the script in the root directory of your Flutter project (same level as `lib`, `pubspec.yaml`, etc.).  
2. Open a terminal in the project root.  
3. Run the script:

```sh
bash widgetbook_setup.sh
```

# Running Widgetbook

1. Once the script is finished and the setup is complete, navigate to the widgetbook directory:

 ```sh
 cd widgetbook  
 ```

2. Run the following command to generate the necessary files:

```sh
dart run build_runner build
```   

3. Now, start Widgetbook using:
   
```sh
flutter run
```

# ⚠️ Important Notice  

During setup, you might see messages about **version conflicts** or **dependency issues**. This happens when some packages in your project require different versions to work together.  

## 🔍 What does this mean?  
- If you see a message like _"Version solving failed"_, it means some dependencies need to be adjusted.  
- The error message usually suggests a fix (e.g., changing a package version).  

## ✅ How to Fix It  
1. Check the error message for suggested version changes.  
2. If a solution is provided (e.g., updating a package version), run the suggested command.  
3. If no suggestion is given, try running:
   
   ```sh
   flutter pub upgrade --major-versions
    ```
4. If the issue persists, manually adjust dependency versions in `pubspec.yaml` and then run:
   
   ```sh
   flutter pub get
   ```

# Contributing

Contributions from users are highly valued and appreciated. Two main ways to contribute to this project are through pull requests and issues.

## Pull Requests

1. Fork the repository and create a branch from the `main` branch.
2. Make changes or additions to the code.
3. Commit the changes, and push them to the branch.
4. Open a pull request to the `main` branch with a clear and concise description of the changes.

## Issues

1. Navigate to the [Issues](https://github.com/GianMen91/gitlab-statistics/issues) section of the repository.
2. Check if there is an existing issue similar to the one you'd like to create.
3. If there isn't an existing issue, create a new issue by clicking the "New issue" button.
4. Provide a descriptive title and detailed information about the proposed changes you want to add to the current script.

---

Feel free to contribute and share

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# Buy me a coffee

<a href="https://www.buymeacoffee.com/giancarlo.mennillo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
