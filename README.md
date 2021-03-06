# UITextFieldValidator

[![Version](https://img.shields.io/cocoapods/v/UITextFieldValidator.svg?style=flat)](http://cocoapods.org/pods/UITextFieldValidator)
[![License](https://img.shields.io/cocoapods/l/UITextFieldValidator.svg?style=flat)](https://github.com/satyerncareer/UITextFieldValidator/blob/master/LICENSE)
[![Platform](https://img.shields.io/cocoapods/p/UITextFieldValidator.svg?style=flat)](http://cocoapods.org/pods/UITextFieldValidator)
[![Language](https://img.shields.io/badge/language-swift%204-green.svg)](https://alamofire.github.io/Alamofire)
## Example
UITextFieldValidator is a UITextField validator which can be use in different ways. So you would now focus on writing your core login and let UITextFieldValidator handle all your field validations. For more you can see "How to use" section bellow.

To run the example project, clone the repo, and run `pod install` from the Example directory first.


## Installation

UITextFieldValidator is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'UITextFieldValidator'
```
## How it works

The validator check your `ContentType` of your UITextField and according to ``ContentType`` it will validate text fields if Content``ContentType`` is set for your text field then it will validate according to your `KeyboardType`. All this take care by this lib.

## How to use
```ruby
import UITextFieldValidator
```

There are two version of validation here, one is for simple validation and second one is validation with range. Range validation will tak two more input for minimum charectors and the maximum charectors

You can pass multiple UITextField in both methods.

Simple validation


```ruby
Validator.shareInstance.textFieldValidator(textField: TextFields...) { (textField, isSuccess) in
    //hand result here
}
```
With range

```ruby
Validator.shareInstance.textFieldValidator(withRange: (textField: TextFields..., minRange: 0, maxRange: 50)) { (textField, isSuccess) in
    //hand result here
}
```
Note :  When all textfield will be validated successfully then textfield will return nil else there will be a textfield which is not validated.

## Author
### Satyendra Chauhan
satyenchauhan5@gmail.com

## License

UITextFieldValidator is available under the MIT license. See the LICENSE file for more info.
