# Android Studio Setup
To be able to debug / repackage / build on the android mobile application, you need to:

- download and install the most recent official IDE for android: [Android Studio](https://developer.android.com/studio/index.html) 

- Verify which version of the JDK you have: open a command line and type javac -version. If the JDK is not available or the version is lower than 1.8, download the [Java SE Development Kit 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html).

> MAC Users : There are, however, known stability issues in Android Studio on Mac when using JDK 1.8. Until these issues are resolved, you can improve stability by downgrading your JDK to an older version (but no lower than JDK 1.6).

- Launch Android Studio after installation.

- Select whether you want to import previous Android Studio settings, then click OK.

---

The Android Studio Setup Wizard guides you through the rest of the setup, which includes downloading Android SDK components that are required for development. 
 We only need SDK 4.4 and above. You can install as many SDK’s packages as you wish to. Note that the packages are huge and therefore precaution must be taken with HDD available space in mind.

![AndroidSDKManager](uploads/images/AndroidSDKManager.png)

###GitHub setting
There are three steps that needs be done before you can make contribution to "take-home" project:

1. Find and fork the "take-home" repository
You can find "take-home" GitHub repository [here](https://github.com/open-learning-exchange/take-home). Fork the repository to your own GitHub account by clicking the fork button (just like what you did in [step 3](http://open-learning-exchange.github.io/#!pages/githubandmarkdown.md#Find_and_fork_the_correct_repository))

2. Clone your own GitHub repository yourGitHubUsername / take-home
In a terminal / console of your choosing, navigate into the working directory of Android studio and git clone your own “take-home“ repository at `https://github.com/yourGitHubUsername/take-home.git`

3. Configure a remote for your local repository
Under your "take-home" directory, type `git remote add upstream https://github.com/open-learning-exchange/take-home.git` so that you can fetch updates from the upstream repository (reference [step 5](http://open-learning-exchange.github.io/#!pages/gitandrepositories.md#Configure_a_remote_for_your_fork))

Now, Run Android studio. Select New from the file menu and select import project.
Navigate to Android studio -> take-home and select the settings.gradle file to import and open the project.

>@todo : 
>http://stackoverflow.com/questions/37397810/android-studio-unable-to-run-avd
>https://www.virtualbox.org/ticket/14294 NB Virtualbox version needs lower equal 4.3.28

- Click on the run button located at the top of your IDE. You will be prompted to Select Deployment Target. Select “Create New Emulator” button.

![AndroidDeploymentTarget](uploads/images/AndroidDeploymentTarget.png)

- Select a device definition from the list provided and click the next button
           
![AndroidHardwareSelection](uploads/images/AndroidHardwareSelection.png)

- Select system image from the list shown. API Level 22 and above works best. Preferably, choose 22 with Android 5.1. Click next to continue.
	
![AndroidMarshmellowSystem](uploads/images/AndroidMarshmellowSystem.png)

- Name the emulator and specify the necessary configuration as shown below. Click on finish to save the emulator. 
	
![AndroidVirtualDevice](uploads/images/AndroidVirtualDevice.png)

- You will be presented with the “Select Deployment Target” dialogue again . Choose the emulator we just created and click on the “OK” button.

![AndroidDeploymentTarget](uploads/images/AndroidDeploymentTarget.png)

- The emulator will be opened with application installed. You have successfully configured the development environment to get you started.
