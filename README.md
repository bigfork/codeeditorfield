# Code Editor Field for SilverStripe 4

Creates an Ace Code Editor (https://ace.c9.io/)

## Installation

`composer require jinjie/codeeditorfield`

## Usage

```php
$fields->push(CodeEditorField::create('MyCode', 'Enter Source Code Here'));
```

## Setting the Programming Language Mode

```php
$fields->push($myCodeEditorField = CodeEditorField::create('MyCode', 'Enter Source Code Here'));

// set mode to html
$myCodeEditorField->setMode('ace/mode/html');
// or javascript
$myCodeEditorField->setMode('ace/mode/javascript');
```
see [resources/thirdparty/ace](resources/thirdparty/ace) for available modes (mode-{language}.js)
