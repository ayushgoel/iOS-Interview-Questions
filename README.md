### Which cannot be retained?

1.) UITableView
2.) NSNumber
3.) NSInteger
4.) NSObject

_Answer: NSInteger_

_Justification_: Not really meant to be a trick question, but helps determine if they understand objects/pointers vs primitive types. 

##### _Potential follow up_: 
 **How might you add an NSInteger to a dictionary or array?**

*Answer: "Box" the value into an NSNumber. (i.e.* **@(1)** *or* **[NSNumber numberWithInteger:1];** *)*

*Justification*: Closely related to why an understanding of objects/primitives is important in day-to-day Obj-C coding.

### In the context of iOS, what is a delegate?

*Rookie college student answer*: It is something you hook up a <something in Interface Builder> to that runs code to create cells/perform an action/etc…

*Jedi Answer*: It is a design pattern leveraging Objective-C protocols used extensively by Apple in iOS. A delegate is simply a pointer to an object that a delegate holder knows how to call. The pattern allows for highly customizable classes and controls with minimum coupling to "owners" of the class or control.

### A block cannot:

1.) Be subclassed
2.) Be retained or released
3.) Access 'self' from the scope in which it is declared
4.) Be passed as an argument

_Answer: Be subclassed_

_Justification_: This one should be pretty trivial to anyone who has even a trivial understanding of blocks, an important Objective-C feature. It also weeds out those who don't know what a block is, which would raise a red flag that a candidate may be a "did the tutorial" iOS developer.

### What is ARC? How does it work?

*Rookie college student answer*: It allows me to write Objective-C code without retain/release.

*Jedi Answer*: It is a compiler feature that uses analysis from the Clang Static Analyzer to automatically insert the proper retain/release calls. This both minimizes the amount of code that needs to be written, as well as helps prevent developer errors.
