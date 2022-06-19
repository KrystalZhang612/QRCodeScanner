# iOS QR Code Scanner
A Simple iOS QR code scanner using Swift UI. <br/>
Jump to:<br/>
[ContentView.swift](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/QRCodeScanner/ContentView.swift)<br/>
[`screenshot 1.1.5`](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.5.png)<br/>
`NOTE`: be aware of the new horizontal line error to internal hyperlink redirecting in Documentations <br/>

# Build
[Setup]()<br/>
[Debugging&Troubleshooting]()<br/>
[Commits&Pushes Steps]()<br/>
[Method Running The Project]()<br/>
[Testing Result]()
# Contribution
[Author]()
# Prerequisite
Developing tool: Xcode `13.4+` Swift, SwiftUI custom dependencies. 
# Compatibility
iPhone 11, iPhone 12, iPhone 13, iPad 10.2+
# Setup
In Xcode IDE, go to info, click to add a Custom iOS Target Properties Key<br/>
Search for Privacy - `Camera Usage Description` <br/>
Value String: “We need the camera to scan the QR code” -> <br/>
This preset will enable users to turn on their camera Privacy for scanning<br/>
<hr>
Secondarily, click to add `Appearance`  Value String: Light -><br/>
If the app is used on a physical device, this functionality will automatically maximize the brightness on the user’s devices for better scannability if QR code is detected. <br/>
<hr>
Next, click File->Add Packages…-> add [CodeScannerDependency](https://github.com/twostraws/CodeScanner) into Package Dependencies.
# Debugging&Troubleshooting
In order to prevent the occurence of 
```swift
“Cannot assign value of type ‘ScanResult’ to type ‘String’ “ error
``` 
at 
```swift 
self.scannedCode = code
```
we need to use 
```swift 
self.scannedCode = code.string 
```
instead to make the value types compatible. <br/>
<hr>
# Commits&Pushes Steps
Must customize commit message for each commit:<br/>
Changes done in ContentView.swift file-> Save -> Source Control->Commit->Flat->Selected the committed file->Enter customized commit message down below->Select Push to Remote (origin/origin/main)-> Commit N files. Done Committing. <br/>
`NOTE`: To retain each commit to Github Repositories: <br/>
Must save -> resume -> rebuild on Simulator -> push both hierarchical and flat modified files and assets remotely to the Github origin/main.
# Method Running The Project
Download the project to local directory<br/>
Xcode must be `13.4` and higher versions<br/>
Compatible with MacOS Monterey `12.0` or higher versions<br/>
Enable Camera access or Local Photo Library access in local device. 
# Testing Result
[Online QR code generator](https://me-qr.com)<br/>
Starting UI that prompts user to scan a QR code to get started: [`screenshot 1.1.6`](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.6.png)<br/>
iOS 15.5 Simulator message. Camera access isn’t available on Xcode Simulator, so select a custom image: [`screenshot 1.1.7`](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.7.png)<br/>
Testing on url link: [screenshot 1.0.7](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.0.7.png)   [screenshot 1.0.8](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.0.8.png)<br/>
Testing on random text:  [screenshot 1.1.0](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.0.png)      [screenshot 1.1.1](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.1.png)<br/>
Testing on image: [screenshot 1.1.2](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.2.png)    [screenshot 1.1.3](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.3.png)        [screenshot 1.1.4](https://github.com/KrystalZhang612/QRCodeScanner/blob/main/screenshot1.1.4.png)<br/>
# Author
Krystal Zhang 
https://github.com/KrystalZhang612
<hr>
*This file was generated by [QRCodeScanner-readme](), on June 18, 2022*
