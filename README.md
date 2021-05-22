# [go back to content](https://github.com/c4arl0s/AppDevelopmentWithSwift#1-getting-started-with-app-development)

# [Building, Running And Debugging An App - Content](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#go-back-to-content)

1. [x] [1. Building and Running](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#1-building-and-running)
2. [x] [2. Using a Personal Device](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#2-using-a-personal-device)
3. [x] [3. Building and Running Wirelessly](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#3-building-and-running-wirelessly)
4. [x] [4. Debugging an Application](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#4-debugging-an-application)
5. [x] [5. Warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#5-warnings)
6. [x] [6. Compile Errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#6-compile-errors)
7. [x] [7. Bugs](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#7-bugs)
8. [x] [8. Lab - Debug your first app](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#8-lab---debug-your-first-app)
    - [x] [Step 1: Find and fix compiler errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-1-find-and-fix-compiler-errors)
    - [x] [Step 2: Find and fix runtime errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-2-find-and-fix-runtime-errors)
    - [x] [Step 3: Find and fix compiler warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-3-find-and-fix-compiler-warnings)

# [Building, Running And Debugging An App](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

# 1. [Building and Running](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

Your first step is to create  a new project in Xcode. You will use the same iOS Single View Application template as in the previous lesson. Name the Project "GettingStarted" and choose a location for saving it.

I will use old pattern When you programming without SceneDelegate.swift file.

Follow the steps according to "[Stop using SceneDelegate swift file](https://github.com/c4arl0s/StopUsingUISceneDelegateSwiftUIXcode115.git)"

Next, you will be presented with the Xcode workspace. Locate the Scheme menu on the Xcode toolbar, then choose the device you want to simulate from the list.

![Screen Shot 2021-03-21 at 5 39 45](https://user-images.githubusercontent.com/24994818/111903425-e1a4a500-8a07-11eb-8551-9cf865ffc266.png)

Click the Run button, or use the keyboard shorcut (Command+R) to begin launching the app in Simulator.

If you are running the app for the first time, Xcode asks whether you would like to enable deverloper mode on your Mac. Develover mode gives Xcode access to certain debugging features without requiring you to enter your password each time. All the lessons in this course assume you have enabled developer mode.

![Screen Shot 2021-03-21 at 5 43 08](https://user-images.githubusercontent.com/24994818/111903528-54158500-8a08-11eb-8251-b2d98c750fc2.png)

After simulator has launched, you should see a device image with a white background. **To rotate the image from portrait to landscape orientation, use the keyboard shortcuts Command-Left Arrow and Command-Right Arrow**.

The Simulator image may appear quite large, depending on the screen resolution of your Mac and the device you chose to simulate. **From inside the Simulator application, you can use keyboard shortcuts, from Command-1 to Command-5, to scale the device image up or down**. If you are using an older Mac, you may want to select an older lower resolution device, such as an iPhone SE, to reduce the total impact of Simulator on your system.

![Screen Recording 2021-03-21 at 5 47 56 2021-03-21 05_53_22](https://user-images.githubusercontent.com/24994818/111903876-c5a20300-8a09-11eb-90f0-4b3a71fcef80.gif)

To quit Simulator, use the keyboard shortcut Command-Q. Or just go back to Xcode.

Simulator does not work for all portions of an App. Certain interactions depend on the actual physical device to run. 

> For example, if you try to use Simulator to test an interaction with the Camera app, the program will crash. If your code depend on other hardware components that don't exist on a Mac - Maybe an accelerometer, a gyroscope, or a proximity sensor - You will want to test with an actual device.

There are also some software limitations with Simulator.

> For example, push notifications can be delivered to physical devices, and the MessageUI framework - which helps compose email and text messages - is incompatible with Simulator. If you are running into a lot of issues in Simulator, you might try testing the code on your iPhone or iPad. Your issues may resolve.

Overall, Simulator works very well when you are developing and debugging apps, but you should always test your code on actual hardware.

# 2. [Using a Personal Device](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

The beauty of mobile apps is that you can take them anywhere. You may find that you want to share your programming progress with friends and coworkers. But before you can begin running your code on a physical device, you must have an account on the Apple Developer website. Accounts are free, so don't worry.

Using a web browser, go to web developer page, and click Account. You can sign up using your existing Apple ID. If you don't have an Apple ID, go ahead and create one - It is also free. Once you have entered your Apple ID, your developer account is good and you can head on back to Xcode.

> A free account enables you to run your iOS apps on only one physical device. If you want to distribute your apps to multiple devices or publish them to the App Store, you will need to enroll in the App Developer Program.

Now you will need to tell Xcode about your new developer account. Open Xcode Preferences using the keyboard shortcut Command-Comma, and select the Accounts button near the upper-left-corner. Click the "+" button in the lower-left corner, and Add Apple ID from the menu. After entering your credentials, you are ready to run and debug apps on a physical iOS device.

![Screen Shot 2021-03-21 at 6 07 13](https://user-images.githubusercontent.com/24994818/111904279-b2903280-8a0b-11eb-804b-72e9c26e3381.png)

Connect your iOS device to your Mac using the appropriate USB cable. Xcode will automatically download the necessary information from the device and will display its  name in the Scheme menu. Choose the name of your physical device - which will typically be at the top of the list, before the device simulators.

Build and run the app again. You may receive the following prompt, asking you to trust the developer certificate. Follow the instructions within the alter to allow the device to run your apps.

![Screen Shot 2021-03-21 at 6 09 39](https://user-images.githubusercontent.com/24994818/111904334-09960780-8a0c-11eb-8e33-40a2a6d22dcd.png)

Build and run once more, and you should see the same simple white screen on your iOS device. To stop the app from running, click the Stop button near the left end of the Xcode toolbar.

# 3. [Building and Running Wirelessly](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

Xcode also gives you the option of deploying an app to your device over your network. To do this, connect your iOS device to your Mac using the appropriate USB cable, and open the Devices and Simulators window by selecting Devices and Simulators from the Window dropdown.

Ensure that your device is selected in the list farthest to the left in the Devices and Simulators window. Check the Connect via network box.

![Screen Shot 2021-03-21 at 6 27 04](https://user-images.githubusercontent.com/24994818/111904854-875b1280-8a0e-11eb-80c3-1c763d0b8833.png)

If your device is on the same network as your Mac, you will see a globe appear next to your device's name within a few moments. This indicates that your device is wirelessly connected.

![Screen Shot 2021-03-21 at 6 29 58](https://user-images.githubusercontent.com/24994818/111904943-def97e00-8a0e-11eb-970f-4a2693e84adb.png)

You can disconnect the USB cable connecting your device to your Mac, and build and run your app wirelessly.

In most cases, the above steps are sufficient for wireless pairing. However, if this does not work for you, you might to be on a corporate or institutional network where the system administrator has put in place certain network restrictions. In this case, simply open the Devices and Simulators window, hold Control and click on your device, then click Connect via IP Address in the dropdown presented. You will then need to find your device's IP address from you device's settings, enter it in the prompt, and click Connect. This should successfully pair your device.

# This was my case

Once you disconnect the device go to Devices and Simulators.

Finding the IP Adress of iOS Devices:

1. Go to Settings > Wi-Fi. If you're not already connected to your network, tap it and connect now.
2. Tap the network's name to open its information.
3. Under the "IPv4 Address" header it should list your IP Address.

Mine was:

Direccion IP: 10.0.0.5

![Screen Shot 2021-03-21 at 6 59 26](https://user-images.githubusercontent.com/24994818/111905789-0f431b80-8a13-11eb-9704-8053b2dda484.png)

Disconnect, build and run again. The connection was successful!!!!. 

# 4. [Debugging an Application](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

Even the best developers struggle to write perfect code. **Debugging is the process of identifying and removing problems that may arise in your app**. Xcode provides tools to help you through this process.

When you run an app as described above, either on the simulator or on your device, Xcode will connect the app to its debugger. This allows you to watch the execution of your code in real time, stop code execution using breakpoints, print information from your code to the console, and much more.

As you proceed through this course, you will encountered three types of issues:

1. Warnings.
2. Compile errors.
3. bugs.

# 5. [Warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

Warnings are the simplest kinds of issues to fix. They are generated whenever your code is built, but they don't prevent your program from successfully compiling and running. Some of the conditions that can throw a warning include:

1. Writing code that never gets executed.
2. Creating a variable that never changes.
3. Using code that is out of date (also known as deprecated code).

Take a look at a warnings. Back in Xcode, select ViewController.swift, in the project navigator and, in the editor area, add the following line of code just below `super.viewDidLoad()`.

```swift
let x = 4
```

This code assigned a value of 4 to a constant named `x`. Build your application using Command-B. You should see a yellow caution sign on the line you just added.

![Screen Shot 2021-03-21 at 8 09 33](https://user-images.githubusercontent.com/24994818/111907907-d019c800-8a1c-11eb-90ce-5f80dfcefcda.png)

Xcode will do its best to explain the warning in a straightforward way:

![Screen Shot 2021-03-21 at 8 11 44](https://user-images.githubusercontent.com/24994818/111907986-17a05400-8a1d-11eb-8d74-9d3f63582724.png)

The compiler is telling you that it created `x` but - Since it is not used in a meaningful way - you can remove it. Delete the line and rebuild to remove the warning.

# 6. [Compile Errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

An error is indicative of a more serious issue.

> For example, invalid code (such as a typo), improperly declaring a variable, or improperly calling a function. Unlike a warning, an error prevents the code from ever being executed. Simulator will not even launch if your code has an error.

Here is a look at two different errors in the making. In ViewController.swift, remove the open and closing parenthesis on the end of `super.viewDidLoad()`, leaving `super.viewDidLoad`. Beneath this line of code, write `navigationController.title = "Debugging"`.

After you build tyhe app, you will see two red error symbols.

![Screen Shot 2021-03-21 at 8 27 26](https://user-images.githubusercontent.com/24994818/111908545-49b2b580-8a1f-11eb-93ed-d7f3330626a0.png)

One of the errors has a dot in the center. Click this eero and Xcode displays a suggestion to fix the code. Click the Fix button to have Xcode implement this suggestion. In this instance, Xcode provides a valid fix. However, the compiler cannot be relied upon the propertly fix all errors - You need to be able to address errors on your own.

The other error has an exclamation point in the center. Xcode does not offer a fix-it for this type of error, but it does provide a message that can help you identify the issue. The compiler expected to see an open and closing parenthesis as the proper syntax for calling a function. Add both characters at the end of `super.viewDidLoad` to remove the last error.

# 7. [Bugs](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

The third type of issue is know as a bug - and it is the hardest issue to track down. A bug is an error that occurs while running the program, resulting in a crash or incorrect output. Finding bugs can involve some time and some real detective work.

in ViewController.swift file, add the following lines of code below `super.viewDidLoad()`:

```swift
override func viewDidLoad() {
    super.viewDidLoad()
    navigationController?.title = "Debugging"
    var names = ["Carlos", "Norma"]
    names.removeFirst()
    names.removeFirst()
    names.removeFirst()
}
```

You may not be familiar with Swift at this point, and that is OK. These lines are simple to understand. `names` is a list containing two pieces of text, "Carlos" and "Norma". Each subsequent line removes the first item from the list. Sice there are three calls to remove the first item, but not only two items in the list, what do you expect will happen?.

Build and run the application. Since the syntax is valid, you will receive the "Build Succeeded" message. Now try running the app. After a few moments, the program will crash, and the following message will be printed to the console.

Console output:

```console
Fatal error: Can't remove first element from an empty collection: file Swift/RangeReplaceableCollection.swift, line 624
2021-03-21 08:38:18.937476-0600 GettingStarted[9744:170279] Fatal error: Can't remove first element from an empty collection: file Swift/RangeReplaceableCollection.swift, line 624
(lldb) 
```

The program crashed when it tried to remove the remaining first element and could not find one. You have already guessed that. But imagine you are unsure how to fix the problem. Xcode can help you to step through the program one line at a time.

Before you start looking for the bug, you will need to add a breakpoint to your code. A breakpoint pauses the execution of a program at a specified point. Create a breakpoint by left-clicking in the gutter area to the left of the line where you want execution to pause. In this case, add the breakpoint to the `var names = ["Carlos", "Norma"]` line.

![Screen Shot 2021-03-21 at 8 45 21](https://user-images.githubusercontent.com/24994818/111909162-ca72b100-8a21-11eb-8619-72f08ab62591.png)

Build and run your app. You will see the program pause at the breakpoint. That is good. In the debug area, show the variables view to inspect the current values. Since the breakpointed line has not yet been executed, `names` contains no values.

Click the "Step over" button to advance execution by one line. In the variables view, you can see that `names` has been assigned the proper values. So far, so good.

![Screen Shot 2021-03-21 at 8 47 49](https://user-images.githubusercontent.com/24994818/111909235-21788600-8a22-11eb-8347-7a5b6bfac023.png)

Click the "Step Over" button again to execute the first call to `names.removeFirst()`. `names` no longer includes "Carlos" in its list, so that worked fine. Click "Step Over" again to execute the second call to `names.removeFirst()`, leaving `names` an empty list with zero values. Still OK. By now, it should be clear that the third call to `names.removeFirst()` is responsible for the bug.

![Screen Shot 2021-03-21 at 8 51 09](https://user-images.githubusercontent.com/24994818/111909358-98ae1a00-8a22-11eb-8f3d-a5493f96e066.png)

Remove the third call to `names.removeFirst()` and run the program again to verify that the error has been fixed.

```swift
override func viewDidLoad() {
    super.viewDidLoad()
    navigationController?.title = "Debugging"
    var names = ["Carlos", "Norma"]
    names.removeFirst()
    names.removeFirst()
}
```

Debugging is a crucial skill for developers to build. When debugging, take the following approach:

1. Try to understand the problem.
2. Brainstorm a potential solution.
3. Try the solution.
4. Verify it worked, repeat as necessary.

Take each bug one step at a time. It can be frustrating to run into bugs when building apps, but it feels great when you are able to fix them.

# 8. [Lab - Debug your first app](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

The objective of this lab is to find and resolve compiler errors, runtime errors, and compiler warnings.

#     - [Step 1: Find and fix compiler errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

1. Open the Xcode project, "FirstTimeDebugging".
2. Try to run the app. Note that i will not run due to a few compiler error.s As you have learned in this lesson, compiler errors are indicated by red symbols in line with the mistake - or where the compiler guesses the mistake might be. All compiler errors are also listed in the issue navigator.

![Screen Shot 2021-03-21 at 9 56 35](https://user-images.githubusercontent.com/24994818/111911563-c350a080-8a2b-11eb-86fe-bc9ac1dd50fd.png)

3. Fix the compiler errors so that you can run the app. Here are two of the more common mistakes that may have caused this app's compiler errors:

 - Missing or extra parentheses or braces (whether opening or closing).
 - Referencing a function or property but with incorrect spelling. (Remember that the compiler is very literal; it expects you to reference a function or property exactly by the name you gave it.
 Hint: Sometimes a single mistake can cause the compiler to flag multiple errors. Fix one mistake and you might eliminate all the error symbols.

Done !

![Screen Shot 2021-03-21 at 10 07 52](https://user-images.githubusercontent.com/24994818/111911997-50482980-8a2d-11eb-86aa-678cc9a0c16e.png)

#     - [Step 2: Find and fix runtime errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

- Were you able to remove all the red error symbols from the project?. If so, try to run the app again.

![Screen Shot 2021-03-21 at 10 12 42](https://user-images.githubusercontent.com/24994818/111912152-fe53d380-8a2d-11eb-8757-5fdcdac0a6e5.png)

- This time around, notice that the app stops execution right after opening in the Simulator and that there is a red line across one of the lines of code on the screen. 

![Screen Shot 2021-03-21 at 10 14 12](https://user-images.githubusercontent.com/24994818/111912194-33602600-8a2e-11eb-879d-7ac8a946e927.png)

- Take a look at the text in the console area to learn what the issue might be. Go ahead and try to solve this runtime error. If it is helpful, you might want to add breakpoints at and before the affected code, then run the app again.

Console output:

```console
Fatal error: Can't remove first element from an empty collection: file Swift/RangeReplaceableCollection.swift, line 624
2021-03-21 10:12:37.843592-0600 FirstTimeDebugging[13222:249176] Fatal error: Can't remove first element from an empty collection: file Swift/RangeReplaceableCollection.swift, line 624
```

Removing the second `removeFirst()` instance method from testArray collection solves the problem.

```swift
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool {
    // Override point for customization after application launch.
    var testArray: [String] = ["Uh oh..."]
    testArray.removeFirst()
    return true
}
```

#     - [Step 3: Find and fix compiler warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)

- Now that the app runs, focus your attention on a few more problems. Open the project's issue navigator. You will note several warnings, indicated by yellow triangles. Address all of these warnings.

```swift
class ViewController: UIViewController {

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
        let sample = "sample"
        print(sample)
        print("Will this line of code ever be reached?")
        someMethod()
    }
    
    func someMethod() {

    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }
    
}
```

![Screen Shot 2021-03-21 at 10 42 52](https://user-images.githubusercontent.com/24994818/111913101-34935200-8a32-11eb-899f-a82d21e92e01.png)