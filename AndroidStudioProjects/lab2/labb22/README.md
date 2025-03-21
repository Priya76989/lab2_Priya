Simple Calculator Flutter App
This is a simple calculator app built using Flutter. The app performs basic arithmetic operations such as addition, subtraction, multiplication, and division. It also uses SharedPreferences to persist the last calculated value even after the app is closed.

Features
Basic arithmetic operations: +, -, *, /
Memory persistence for the last calculated value using SharedPreferences
Error handling for division by zero
Limit input to 8 digits
Clear Entry (CE) and Clear (C) functionalities
Requirements
Flutter SDK (version 2.0 or above)
Dart SDK (version 2.12 or above)
Setup
Clone the repository or download the project files.

bash
Copy
Edit
git clone https://github.com/your-repo/simple-calculator-flutter.git
Navigate to the project directory.

bash
Copy
Edit
cd simple-calculator-flutter
Install the necessary dependencies.

bash
Copy
Edit
flutter pub get
Run the app.

bash
Copy
Edit
flutter run
How It Works
Main Function: The app initializes SharedPreferences to retrieve the last calculated value and passes it to the CalculatorApp.

CalculatorApp: This is the root widget that sets up the theme and passes the lastValue to the CalculatorScreen.

CalculatorScreen: This stateful widget holds the logic for the calculator, including handling digit and operator presses, performing calculations, and updating the display.

SharedPreferences: The last result is stored using SharedPreferences to allow persistence even after restarting the app.

Features Breakdown
Digits: Buttons for digits (0-9) allow the user to input numbers.

Operators: Buttons for +, -, *, and / perform basic arithmetic operations.

Equals Button: After entering an operation, the user can press = to compute the result.

Clear and Clear Entry: The C button resets the entire calculation, while CE clears the current input.

Example Screenshot
(Here, you can add an image or screenshot of your app running)

Troubleshooting
SharedPreferences: Ensure that you have the shared_preferences package added in your pubspec.yaml file.

yaml
Copy
Edit
dependencies:
  shared_preferences: ^2.0.15
