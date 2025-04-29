
# Boilerplate  
  
This project is a boilerplate for a new Flutter application. It provides a structured starting point for developing cross-platform mobile applications using Flutter. The project includes a well-organized folder structure, essential configurations, and sample code to help developers quickly set up and start building their applications.  
  
### Key Features  
  
- Modular Architecture: The codebase is organized into modules for UI, widgets, models, dependency injection, stores, utilities, constants, and data management.  
- Localization: Includes support for multiple languages with JSON files for different locales.  
- Theming: Provides a theme store for managing application themes.  
- Network Handling: Contains network modules and utilities for making API calls and handling network exceptions.  
- State Management: Uses MobX for state management with generated store files.  
- Dependency Injection: Implements a service locator pattern for managing dependencies.  
- Custom Widgets: Includes reusable custom widgets like buttons, text fields, and progress indicators.  
- Sample Screens: Provides sample screens for login, splash, and home pages.  
- Assets Management: Organized assets for icons, fonts, images, and localization files.  
  
## Getting Started  
  
This project is a starting point for a Flutter application.  
  
### Prerequisites  
  
- Flutter SDK: [Install Flutter](https://flutter.dev/docs/get-started/install)  
- Dart SDK: Included with Flutter  
- Android Studio or Visual Studio Code: [Install Android Studio](https://developer.android.com/studio) or [Install VS Code](https://code.visualstudio.com/)  
  
### Installation  
  
1. Clone the repository:  
   ```  
   git clone git@github.com:Shahzeb-99/flutter-boilerplate.git  
   cd flutter-boilerplate  
   ```  
  
2. Get the dependencies:  
   ```  
   flutter pub get  
   ```  
  
### Running the App  
  
1. Connect a device or start an emulator.  
2. Run the app:  
   ```  
   flutter run  
   ```  
  
### Building the App  
  
To build the app for release:  
```  
flutter build apk  
```  
  
## Project Structure  
  
- `lib/`: Contains the Dart source code.  
- `android/`: Contains the Android-specific code.  
- `ios/`: Contains the iOS-specific code.  
- `test/`: Contains the unit and widget tests.  
  
## Folder Structure  
  
```  
flutter-boilerplate/  
├── android/  
├── ios/  
├── lib/  
│   ├── ui/  
│   │   ├── login/  
│   │   │   └── login.dart  
│   │   ├── splash/  
│   │   │   └── splash.dart  
│   │   ├── home/  
│   │   │   └── home.dart  
│   │   ├── my_app.dart  
│   ├── widgets/  
│   │   ├── progress_indicator_widget.dart  
│   │   ├── empty_app_bar_widget.dart  
│   │   ├── rounded_button_widget.dart  
│   │   ├── app_icon_widget.dart  
│   │   └── textfield_widget.dart  
│   ├── models/  
│   │   ├── language/  
│   │   │   └── Language.dart  
│   │   ├── post/  
│   │       ├── post.dart  
│   │       └── post_list.dart  
│   ├── di/  
│   │   ├── module/  
│   │   │   ├── local_module.dart  
│   │   │   └── network_module.dart  
│   │   └── components/  
│   │       └── service_locator.dart  
│   ├── stores/  
│   │   ├── theme/  
│   │   │   ├── theme_store.dart  
│   │   │   └── theme_store.g.dart  
│   │   ├── form/  
│   │   │   ├── form_store.dart  
│   │   │   └── form_store.g.dart  
│   │   ├── language/  
│   │   │   ├── language_store.dart  
│   │   │   └── language_store.g.dart  
│   │   ├── user/  
│   │   │   ├── user_store.dart  
│   │   │   └── user_store.g.dart  
│   │   ├── post/  
│   │   │   ├── post_store.dart  
│   │   │   └── post_store.g.dart  
│   │   └── error/  
│   │       ├── error_store.dart  
│   │       └── error_store.g.dart  
│   ├── utils/  
│   │   ├── locale/  
│   │   │   └── app_localization.dart  
│   │   ├── dio/  
│   │   │   └── dio_error_util.dart  
│   │   ├── device/  
│   │   │   └── device_utils.dart  
│   │   ├── routes/  
│   │   │   └── routes.dart  
│   │   └── encryption/  
│   │       └── xxtea.dart  
│   ├── constants/  
│   │   ├── font_family.dart  
│   │   ├── app_theme.dart  
│   │   ├── colors.dart  
│   │   ├── assets.dart  
│   │   ├── dimens.dart  
│   │   └── strings.dart  
│   ├── data/  
│   │   ├── network/  
│   │   │   ├── exceptions/  
│   │   │   │   └── network_exceptions.dart  
│   │   │   ├── rest_client.dart  
│   │   │   ├── apis/  
│   │   │   │   └── posts/  
│   │   │   │       └── post_api.dart  
│   │   │   ├── constants/  
│   │   │   │   └── endpoints.dart  
│   │   │   └── dio_client.dart  
│   │   ├── repository.dart  
│   │   ├── sharedpref/  
│   │   │   ├── shared_preference_helper.dart  
│   │   │   └── constants/  
│   │   │       └── preferences.dart  
│   │   └── local/  
│   │       ├── datasources/  
│   │       │   └── post/  
│   │       │       └── post_datasource.dart  
│   │       └── constants/  
│   │           └── db_constants.dart  
│   └── main.dart  
├── assets/  
│   ├── icons/  
│   │   ├── ic_launcher.png  
│   │   └── ic_appicon.png  
│   ├── fonts/  
│   │   ├── Product-Sans-Italic.ttf  
│   │   ├── Product-Sans-Regular.ttf  
│   │   ├── Product-Sans-Bold-Italic.ttf  
│   │   └── Product-Sans-Bold.ttf  
│   ├── lang/  
│   │   ├── en.json  
│   │   ├── es.json  
│   │   └── da.json  
│   └── images/  
│       ├── img_no_jobs.png  
│       └── img_login.jpg  
├── linux/ 
├── macos/ 
├── web/ 
├── test/  
│   └── widget_test.dart  
├── pubspec.yaml  
├── pubspec.lock  
├── analysis_options.yaml  
├── .gitignore  
├── .metadata  
├── .fvmrc  
└── README.md  
```  

  
## Contributing  
  
1. Fork the repository.  
2. Create a new branch (`git checkout -b feature-branch`).  
3. Make your changes.  
4. Commit your changes (`git commit -m 'Add some feature'`).  
5. Push to the branch (`git push origin feature-branch`).  
6. Open a pull request.  
  
