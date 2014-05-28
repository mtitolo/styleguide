# reddit iOS styleguide

## General Style

Follow the [Apple Cocoa Guidelines](https://developer.apple.com/library/mac/documentation/Cocoa/Conceptual/CodingGuidelines/CodingGuidelines.html) as a primary source. Anything not covered in that doc should follow the [NYT iOS Styleguide](https://github.com/NYTimes/objective-c-style-guide).  

Also, make sure to `Treat Warnings as Errors` and keep your Xcode up to date.

## Classes and Files
Categories and subclasses should live as their own individual files. Multiple categories/classes should not be grouped together into one class. Whenever possible, name things the same as they are on the server.  

The file system should mimick the structure in Xcode wherever possible. This just makes projects easier to manage.

## Dependencies
Check in the `Pods` folder. Always use a Pod if one is available. If one isn't note it in the project's README as a special setup step. Specify versions using `'~> X.X.X'` in the Podfile.  

## Leave the code better than you found it
If something doesn't follow these guidelines, fix it. Find a small bug? Fix it. See something that should be shared? Share it.