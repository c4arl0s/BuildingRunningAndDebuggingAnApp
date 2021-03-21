# [go back to content](https://github.com/c4arl0s/AppDevelopmentWithSwift#1-getting-started-with-app-development)

# [Building, Running And Debugging An App - Content](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#go-back-to-content)

1. [Building and Running](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#1-building-and-running)
2. [Using a Personal Device](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#2-using-a-personal-device)
3. [Building and Running Wirelessly](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#3-building-and-running-wirelessly)
4. [Debugging an Application](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#4-debugging-an-application)
5. [Warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#5-warnings)
6. [Compile Errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#6-compile-errors)
7. [Bugs](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#7-bugs)
8. [Lab - Debug your first app](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#8-lab---debug-your-first-app)
    - [Step 1: Find and fix compiler errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-1-find-and-fix-compiler-errors)
    - [Step 2: Find and fix runtime errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-2-find-and-fix-runtime-errors)
    - [Step 3: Find and fix compiler warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#--step-3-find-and-fix-compiler-warnings)

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
# 3. [Building and Running Wirelessly](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 4. [Debugging an Application](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 5. [Warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 6. [Compile Errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 7. [Bugs](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 8. [Lab - Debug your first app](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 1: Find and fix compiler errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 2: Find and fix runtime errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 3: Find and fix compiler warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)