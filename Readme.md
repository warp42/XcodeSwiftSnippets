#Xcode Swift Code Snippets

I want to present you some convenient code snippets I gathered recently for Swift.
As [Swift](https://developer.apple.com/swift/) becomes more and more popular, it gains [CocoaPods support](http://blog.cocoapods.org/Pod-Authors-Guide-to-CocoaPods-Frameworks/) and probably more and more people will be using it.

##Inspiration
I was inspired by Matt Thompson's [Xcode-Snippets](https://github.com/mattt/Xcode-Snippets) article and GitHub repo but I haven't found anything similar for Swift.

I also used [that thing in swift](https://thatthinginswift.com) and [SwiftSingleton](https://github.com/hpique/SwiftSingleton) as a sample implementations.

##How to import all code snippets to Xcode
All Xcode code snippets exist as a `.plist` files in `~/Library/Developer/Xcode/UserData/CodeSnippets/`
You can simply copy all code snippets from `plist` directory in this repo into this folder, restart Xcode and you should have all of them ready to use.

Note: Create the folder if the folder doesn't exist already. It is created by Xcode when user adds their first cusom snippet.

##Usage
I named all of snippets using scheme `Swift ...` and set all Completion Shortcuts to `swift-...` so each time you type `swift` in code editor you should see all snippets you can use in that place.

![Xcode use Swift code snippets](https://raw.githubusercontent.com/burczyk/XcodeSwiftSnippets/master/assets/xcode-use-code-snippet-2.gif)

##How to create your own snippets
To add code snippet to Xcode show **Utilities** right panel and press `{}` button (*Show the Code Snippet library*) in lower panel.
Then select a code you would like to treat as a snippet, press and hold a left mouse button for a while and drag whole selection to the right panel (if you drag to early you'll probably only deselect text; you can also try dragging from a whitespace instead of the letter).

![Xcode create code snippet](https://raw.githubusercontent.com/burczyk/XcodeSwiftSnippets/master/assets/xcode-add-code-snippet-2.gif)

###Placeholder tokens
If you want to add this nice placeholder in rounded blue rect simply put it between `<#` and `#>` and it will be transformed in both editor and final snippet.

##Snippets
Currently existing snippets (I hope they will be updated on a regular basis with your help :) ):

```
0ADC5D4B... :[swift-uiremotenotification] UIRemoteNotification registration and handling snippet for Swift
1528A53D... :[swift-closureoptionaltypealias] Optional closure typealiast with arguments and return value snippet for Swift
183B54E8... :[swift-uitableviewdelegate] UITableViewDelegate snippet for Swift
3165F25A... :[swift-message] MFMessageComposeViewController snippet for Swift
380DBCD1... :[swift-uitableviewdatasource] UITableViewDataSource snippet for Swift
42AA2BDB... :[swift-closuretypealias] Closure typealias with arguments and return value snippet for Swift
449FB7DE... :[swift-mail] MFMailComposeViewController snippet for Swift
5871FA36... :[swift-uicollectionviewdatasource] UICollectionViewDataSource snippet for Swift
695424DE... :[swift-uicollectionviewdelegate] UICollectionViewDelegate snippet for Swift
731C3867... :[swift-dispatchasync] GCD dispatch_async snippet for Swift
7D773810... :[swift-uiviewconvrollerlifecycle] UIViewController lifecycle snippet for Swift
B005E7A7... :[swift-sortarrayofstrings] 
DA8B025D... :[swift-didbecomeactive] UIApplicationDidBecomeActiveNotification observer snippet for Swift
DAA936A9... :[swift-singleton] Singleton pattern using nested struct in Swift
E3AE2218... :[swift-documentdirectory] Document directory path snippet for Swift
E772ABB6... :[swift-dispatchafter] GCD dispatch_after snippet for Swift
E8847AF3... :[swift-dispatchmain] GCD dispatch_async on main queue snippet for Swift
F60D36B3... :[swift-nslocalizedstring] NSLocalizedString function snippet for Swift
```


##More snippets?
This is a good start but I encourage you to create your own snippets or correct existing ones and create Pull Requests. Please provide plain snippet as `.swift` source code as well as its `.plist` counterpart so it can be easily imported.
You can use `plist/generate_list.py` script to generate snippets list by running: `python generate_list.py`.

##Do you like it?
Do you like this repo? Share it on Twitter, Facebook, Google+ or anywhere you like so that more of us can use it and help. Thanks!
