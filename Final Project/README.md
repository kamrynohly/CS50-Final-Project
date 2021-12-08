Kamryn Ohly
CS50 Final Project
December 7, 2021
Harvard WECode iOS

Check out the video demonstration here:
[Youtube Video](https://youtu.be/48Yr_BxkBNo)

# Introduction

Hello, world! Thank you so much for taking the time to review my CS50 final project, where I have created the app Harvard WECode for iOS devices. This app is meant to be used by attendees of Harvard WECode's Undergraduate Conference at the SEC from February 18-20, 2022.

As a member of the Harvard WECode board, we are incredibly excited to put on a massive conference event, yet the organization of such a large event is both wildly detail-oriented and difficult for both our board, and for our attendees! With the creation of this app, I hope to help consolidate the large amounts of information that we offer to our attendees into an easy to navigate platform. Overall, the app has the goal of letting everyone know what WECode has to offer - in a way that isn't overwhelming!

Additionally, I wanted to create a platform for users to interact with each other as they attend the conference in order to help build an enduring community. While platforms like Slack/Discord exist, I believe that having a WECode-centered app that includes a chat feature like these platforms would be a better connector of attendees, as they can share and discuss events live. Rather than having to flip between apps or pages in a book, they can all use the same one! 

Thus, the Harvard WECode iOS App was born!

## Viewing the App: Required Components

Check out the video demonstration here:
[Youtube Video](https://youtu.be/48Yr_BxkBNo)
Link: https://youtu.be/48Yr_BxkBNo

In order to run the Harvard WECode project, you must have access to an Apple computer, as it is an iOS-based project. Once you are on the Apple/Mac, then you must install Apple's iOS-app builder: Xcode. You can find and install Xcode from the App Store on your Apple device. Do be warned - it sadly requires around 40-50GB of available space to perform the installation (although it will not take the entirety of this space). 

Once Xcode is installed, you can download/open the folder called HarvardWECode that is directly inside of my project folder. Once inside of this folder, you will see a list of other folders and files. Open the file called 

HarvardWECode.xcworkspace

and it should open automatically in Xcode. A quick note: this file should have a white background with the Xcode logo, do NOT open the file with the blue background, or it may cause issues with the simulation of the project.

Once you are viewing the .xcworkspace file with Xcode, then continue to the next section.

## Viewing the App: Simulating the App in Xcode

Next, we want to simulate the project on an iOS device, which luckily Xcode enables us to do! 

On the top of Xcode, the middle of the screen should have a pink/red logo of the app, followed by a device to simulate the project on. Click on the device selected and be sure to select the iPhone 11 under the list of available simulators. 

Once the iPhone 11 Simulator is selected, the top of the far left-pane of Xcode should have a play button. To run the simulator and open the app, click the play button and wait for the simulator to automatically open. This will likely take a few minutes as the packages build and the simulator starts.

When the simulator opens, it should load onto the opening screen of the Harvard WECode app. At this point, we can begin at the next section.

## Operating the App

Now! The best part of the project - utilizing it! Once the app is loaded onto the simulator, you should be seeing the opening screen with the Harvard WECode logo. This screen has two buttons: one to login and one to register an account. If this is your first time using the application, use your mouse over the button on the simulator to click the Register button. If you have an account, select the Sign-In button. If you misclick, no worries! Simply click the back buttons on the top left of the page.

Now, you can fill out the form respectively with your information, and when completed, click Register or Sign-In.

This should take you to the For You page of the application. From this point, you will have access to a tab-bar with the following options: For You, Interact, Schedule, and Profile. 

The For You page does not require any engagement by the user. It will be updated with notifications from the WECode Board team during the conference with messages.

The Interact page offers users a chance to view messages in three sections: Q&A, Chat, and Resources. Simply tap the segmented control (the three sliders), and the messages should load automatically. To reply to a message, you can tap reply, respond at the bottom of the page, and click Post to save your message. Additionally, you can send your own message into a chat by selecting the chat, then clicking the + button on the top right of the screen. It should pop up with a text-field for your message that you can submit!

On the Schedule page, you can view the WECode schedule for each day of the conference by selecting the date on the slider, then scrolling up and down through the events. Friday only has one event, so no scrolling is necessary, and the following two days will automatically update with changes!

Lastly, on the Profile page, you should start out with a relatively empty account. As your first order of business, select the Edit account button above the tab-bar, then you can add a picture, a short bio about yourself, and two links to social media accounts (one of your choice as well as LinkedIn). Be sure to copy and paste the entire link, not just the name of your account. After you have completed this, click Save. Your changes may take a bit of time to load. 

Also on the Profile page, if you meet a new friend at the conference of whom you would like to stay in touch, click on one of the Connect buttons on your Profile page. It should take you to a page where your friend can scan a custom barcode for the link you provided when you edited your account. Then, you can click the back button and continue navigating through the page.

Lastly, to logout of your account, select the Log Out button on your Profile page tab, and agree to the Log Out alert.

This should return you to the beginning, and you can continue as you may wish!

Lastly, to stop the simulation of the project, navigate to Xcode and click the square Stop button next to the button that you clicked to begin the simulation. This should close any running code.

## Thank you! Happy coding!