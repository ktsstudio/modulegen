# modulegen
A template based cocoapods module code generator for iOS projects

## Install

Clone or download the repository and run:

```shell
git clone https://github.com/ktsstudio/modulegen.git
cd modulegen
sudo make install 
```

## Usage

Help:
```shell
modulegen --help
```

Generate default module for using with UIKit, KMP ViewModel and BaseVmViewController<ViewModel, View> with specific podspec file:
```shell
modulegen [module-name] [file-name]
```

Generate module for using with SwiftUI, KMP ViewModel and BaseSUIVmViewController<ViewModel, SUIView> with specific podspec file:
```shell
modulegen [module-name] [file-name] --sui
```

Generate module for using with UIKit, without KMP ViewModel and without base ViewController class with specific podspec file:
```shell
modulegen [module-name] [file-name] --novm
```

Generate module for using with SwiftUI, without KMP ViewModel and without base ViewController class with specific podspec file:
```shell
modulegen [module-name] [file-name] --sui --novm
```

Examples
```shell
# examples
modulegen feature-journal-details JournalDetails
modulegen feature-journal-details JournalDetails --sui
modulegen feature-journal-details JournalDetails --novm
modulegen feature-journal-details JournalDetails --sui --novm
```
