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
# 5. [Warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 6. [Compile Errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 7. [Bugs](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
# 8. [Lab - Debug your first app](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 1: Find and fix compiler errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 2: Find and fix runtime errors](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)
#     - [Step 3: Find and fix compiler warnings](https://github.com/c4arl0s/BuildingRunningAndDebuggingAnApp#building-running-and-debugging-an-app---content)