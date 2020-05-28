# Xcode OSAX template

## Xcode project template that builds a scripting addition

First, a historical note: I created this mostly out of curiosity for how to build a third-party scripting addition for AppleScript, and it taught me a lot. Nevertheless, you very likely have little to no use for this, as third-party scripting additions are all but dead as of macOS 10.14.

Regardless, here is the original text of this repo's README:

This template revives the ancient art of writing Scripting Additions for AppleScript and the OSA. While it has been done before, there aren't many examples to go by, and only one of these examples is open source (that I know of; they're pretty hard to find). In addition, many of the vital resources that cover using Carbon APIs (still required for most things OSA) have been hidden or wiped entirely from Apple's Developer website. Finally, a lot of the old AppleScript communities that people used to share their stuff on are largely gone or no longer updated with the latest info (osaxen.com in particular). This makes getting off your feet with an OSA Scripting Addition bundle pretty tough. There _is still_ enough material out there to learn how to make one; it's just pretty tough to find. I'm here to help you with that.

This template provides a starting point for writing scripting additions for the OSA. It includes a predefined convenience macro for Apple Event handler functions that you would otherwise have to go digging deep into some old documents to find. It includes one very simple, yet fully functioning Event handler that gives you a starting point for writing your own code. And finally, this template takes care of all the annoying quirks about 'aete' resources and whatnot carried over from the Classic Mac OS, by including the extra Build Phases required to make a Scripting Addition functional.

You will still have to read some old documents to know how to do more than return true or false, but lucky for you, I'll hook you up with just what you need: [applescriptlibrary.wordpress.com](http://applescriptlibrary.wordpress.com) (Website not made by me). You're welcome! In particular, make sure to check out the Apple Events Programming Guide. Also, [this technote](https://developer.apple.com/library/mac/technotes/tn1164/_index.html#//apple_ref/doc/uid/DTS10003003) covers specifically the topic of scripting additions, in particular the 10.6 Info.plist scheme for defining handlers. As well, [AppleScript Overview](https://developer.apple.com/library/content/documentation/AppleScript/Conceptual/AppleScriptX/AppleScriptX.html#//apple_ref/doc/uid/10000156-BCICHGIE) provides good general information on the OSA and its supporting mechanisms, and is a good read. Finally, the section "Preparing a Scripting Definition File" in [Cocoa Scripting Guide](https://developer.apple.com/library/content/documentation/Cocoa/Conceptual/ScriptableCocoaApplications/SApps_creating_sdef/SAppsCreateSdef.html#//apple_ref/doc/uid/TP40001979) contains extremely handy information on writing your sdef file. Not everything you can do with an sdef is here, though; be sure to read the XML DTD, check out `man 5 sdef` or look up a tutorial (information on sdefs is plentiful, because they're what _everybody_ uses to make their Cocoa apps scriptable).
