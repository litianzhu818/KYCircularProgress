KYCircularProgress
==================

Flexible progress bar written in Swift.

## Features
- [x] Gradation Color
- [x] Progress Closure
- [x] UIBezierPath Progress Bar

## Demo
<p align="center" >
<img src="http://kentya6.github.io/KYCircularProgress/demo.gif" width="318" height="509"/>
</p>

## Requirement
* iOS7.0+
* Xcode6.0.1+

## Usage
#### Create KYCircularProgress
```swift
var circularProgress: KYCircularProgress! = KYCircularProgress(frame: self.view.bounds)
```

#### Gradation Color
```swift
// support Hex color to RGB color
circularProgress.colors = [0xA6E39D, 0xAEC1E3, 0xE1A5CB, 0xF3C0AB]
```

#### Progress Closure
```swift
circularProgress.progressChangedClosure({ (progress: Double, circularView: KYCircularProgress) in
	println("progress: \(progress)")
})
```

#### UIBezierPath Progress Bar
```swift
// create "Star progress bar"
let path = UIBezierPath()
path.moveToPoint(CGPointMake(50.0, 2.0))
path.addLineToPoint(CGPointMake(84.0, 86.0))
path.addLineToPoint(CGPointMake(6.0, 33.0))
path.addLineToPoint(CGPointMake(96.0, 33.0))
path.addLineToPoint(CGPointMake(17.0, 86.0))
path.closePath()
circularProgress.path = path
```
## Installation
1. Add `KYCircularProgress.swift` in your project.

## Licence

The MIT License (MIT)

Copyright (c) 2014 Kengo YOKOYAMA

## Author

[kentya6](https://github.com/kentya6)