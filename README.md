# IOS-16-Learning
IOS 16 ----> This repo contains the files and projects that i have played around while learning IOS 16 it was just a Quick refreshment over the top to my Previous Ios  knowledge 

Links for learning ---> 
1. https://developer.apple.com/swift/
(documentation 😌)

2. yt channels 
 https://www.youtube.com/@iosmayank/videos (IOS Mayank / swift anywhere)
 https://www.youtube.com/@seanallen (Sean allen ) MY FAV 😄
 https://www.youtube.com/@HiteshChoudharydotcom (IronMan of Development world hiteshchoudhary Sir //  https://github.com/hiteshchoudhary)

  there are many more wonderFull content creators out there do check them out and comit out there names as well 
  
  3. Software Required Xcode that's it and most Important Consistency 😃
   https://apps.apple.com/in/app/xcode/id497799835?mt=12
  
  
  
  About Swift ----> (Source Apple website)
  
Swift
OverviewResources
Watch sessions about Swift from WWDC22

Swift
The powerful programming language that is also easy to learn.
Swift is a powerful and intuitive programming language for iOS, iPadOS, macOS, tvOS, and watchOS. Writing Swift code is interactive and fun, the syntax is concise yet expressive, and Swift includes modern features developers love. Swift code is safe by design and produces software that runs lightning-fast.

Modern
Designed for safety
Fast and powerful
Great first language
Open source
Playgrounds and Read-Eval-Print-Loop (REPL)
Package manager
Objective-C interoperability
Modern
Swift is the result of the latest research on programming languages, combined with decades of experience building Apple platforms. Named parameters are expressed in a clean syntax that makes APIs in Swift even easier to read and maintain. Even better, you don’t even need to type semi-colons. Inferred types make code cleaner and less prone to mistakes, while modules eliminate headers and provide namespaces. To best support international languages and emoji, Strings are Unicode-correct and use a UTF-8 based encoding to optimize performance for a wide-variety of use cases. Memory is managed automatically using tight, deterministic reference counting, keeping memory usage to a minimum without the overhead of garbage collection. You can even write concurrent code with simple, built-in keywords that define asynchronous behavior, making your code more readable and less error-prone.


Perform powerful custom transformations using streamlined closures.

These forward-thinking concepts result in a language that’s fun and easy to use.

Swift has many other features to make your code more expressive:

Generics that are powerful and simple to use
Protocol extensions that make writing generic code even easier
First class functions and a lightweight closure syntax
Fast and concise iteration over a range or collection
Tuples and multiple return values
Structs that support methods, extensions, and protocols
Enums can have payloads and support pattern matching
Functional programming patterns, e.g., map and filter
Built-in error handling using try / catch / throw
Designed for safety
Swift eliminates entire classes of unsafe code. Variables are always initialized before use, arrays and integers are checked for overflow, memory is automatically managed, and enforcement of exclusive access to memory guards against many programming mistakes. Syntax is tuned to make it easy to define your intent — for example, simple three-character keywords define a variable ( var ) or constant ( let ). And Swift heavily leverages value types, especially for commonly used types like Arrays and Dictionaries. This means that when you make a copy of something with that type, you know it won’t be modified elsewhere.

Another safety feature is that by default Swift objects can never be nil. In fact, the Swift compiler will stop you from trying to make or use a nil object with a compile-time error. This makes writing code much cleaner and safer, and prevents a huge category of runtime crashes in your apps. However, there are cases where nil is valid and appropriate. For these situations Swift has an innovative feature known as optionals. An optional may contain nil, but Swift syntax forces you to safely deal with it using the ? syntax to indicate to the compiler you understand the behavior and will handle it safely.

extension Collection where Element == Player {
    // Returns the highest score of all the players,
    // or `nil` if the collection is empty.
    func highestScoringPlayer() -> Player? {
        return self.max(by: { $0.highScore < $1.highScore })
    }
}
Use optionals when you might have an instance to return from a function, or you might not.

if let bestPlayer = players.highestScoringPlayer() {
    recordHolder = """
        The record holder is \(bestPlayer.name),\
        with a high score of \(bestPlayer.highScore)!
        """
} else {
    recordHolder = "No games have been played yet."
}
print(recordHolder)
// The record holder is Erin, with a high score of 271!

let highestScore = players.highestScoringPlayer()?.highScore ?? 0
// highestScore == 271
Features such as optional binding, optional chaining, and nil coalescing let you work safely and efficiently with optional values.

Fast and powerful
From its earliest conception, Swift was built to be fast. Using the incredibly high-performance LLVM compiler technology, Swift code is transformed into optimized machine code that gets the most out of modern hardware. The syntax and standard library have also been tuned to make the most obvious way to write your code also perform the best whether it runs in the watch on your wrist or across a cluster of servers.

Swift is a successor to both the C and Objective-C languages. It includes low-level primitives such as types, flow control, and operators. It also provides object-oriented features such as classes, protocols, and generics, giving Cocoa and Cocoa Touch developers the performance and power they demand.

Great first language
Swift can open doors to the world of coding. In fact, it was designed to be anyone’s first programming language, whether you’re still in school or exploring new career paths. For educators, Apple created free curriculum to teach Swift both in and out of the classroom. First-time coders can download Swift Playgrounds—an app for iPad that makes getting started with Swift code interactive and fun.

Aspiring app developers can access free courses to learn to build their first apps in Xcode. And Apple Stores around the world host Today at Apple Coding & Apps sessions where you can get practical experience with Swift code.

Learn more about Swift education resources from Apple

Open source
Swift is developed in the open at Swift.org, with source code, a bug tracker, forums, and regular development builds available for everyone. This broad community of developers, both inside Apple as well as hundreds of outside contributors, work together to make Swift even more amazing. There is an even broader range of blogs, podcasts, conferences and meetups where developers in the community share their experiences of how to realize the great potential of Swift.

Cross platform
Swift already supports all Apple platforms and Linux, with community members actively working to port to even more platforms. With SourceKit-LSP, the community is also working to integrate Swift support into a wide-variety of developer tools. We’re excited to see more ways in which Swift makes software safer and faster, while also making programming more fun.

Swift for server
While Swift powers many new apps on Apple platforms, it’s also being used for a new class of modern server applications. Swift is perfect for use in server apps that need runtime safety, compiled performance and a small memory footprint. To steer the direction of Swift for developing and deploying server applications, the community formed the Swift Server work group. The first product of this effort was SwiftNIO, a cross-platform asynchronous event-driven network application framework for high performance protocol servers and clients. It serves as the foundation for building additional server-oriented tools and technologies, including logging, metrics and database drivers which are all in active development.

To learn more about the open source Swift community and the Swift Server work group, visit Swift.org

Playgrounds and Read-Eval-Print-Loop (REPL)
Much like Swift Playgrounds for iPad, playgrounds in Xcode make writing Swift code incredibly simple and fun. Type a line of code and the result appears immediately. You can then Quick Look the result from the side of your code, or pin that result directly below. The result view can display graphics, lists of results, or graphs of a value over time. You can open the Timeline Assistant to watch a complex view evolve and animate, great for experimenting with new UI code, or to play an animated SpriteKit scene as you code it. When you’ve perfected your code in the playground, simply move that code into your project. Swift is also interactive when you use it in Terminal or within Xcode’s LLDB debugging console. Use Swift syntax to evaluate and interact with your running app, or write new code to see how it works in a script-like environment.

Package manager
Swift Package Manager is a single cross-platform tool for building, running, testing and packaging your Swift libraries and executables. Swift packages are the best way to distribute libraries and source code to the Swift community. Configuration of packages is written in Swift itself, making it easy to configure targets, declare products and manage package dependencies. Swift packages can also include custom commands that help build your projects and provide additional tooling. Swift Package Manager itself is actually built with Swift and included in the Swift open source project as a package.

Objective-C interoperability
You can create an entirely new application with Swift today, or begin using Swift code to implement new features and functionality in your app. Swift code co-exists along side your existing Objective-C files in the same project, with full access to your Objective-C API, making it easy to adopt.

Get started
Download Xcode and learn how to build apps using Swift with documentation and sample code.


