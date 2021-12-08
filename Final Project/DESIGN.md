Kamryn Ohly
CS50 Final Project
December 7, 2021
Harvard WECode iOS

Check out the video demonstration here:
[Youtube Video](https://youtu.be/48Yr_BxkBNo)

# Introduction of Tech Used

Hello, world! For this project, I utilised the language of Swift and program Xcode to create the iOS app for Harvard WECode. Additionally, I used Firebase hosted by Google to create my database for the project, implementing Cocoapods inside of my Xcode project to install necessary components.

## Overall Design of App

For this app, I began designing the UI/UX first, as I needed the proper layout of my app to be friendliest to its users before I could begin coding. I decided to implement the user registration and login pages, and then stuck with the tab-bar controller for the rest of the features of the app. My intention was that consolidating the offerings of the WECode conference into four main pages, followed by smaller pages that branch from the four main ones, would be easiest to navigate. I created the appearances of the pages, including the buttons, labels, tables, and views, first. From that point, I began working on installing the necessary packages that I would need to begin coding.

I began by using Cocoapods to install Firebase and its dependencies, as I would use Firebase's Authentication, Database, and Storage to navigate the app. Through Firebase, I am able to store the information about users, the app's images, and the overall data of the application on Google, so then they are accessible at all times. I also chose Firebase, as it allows for the WECode board to have hands-on and visual access to our information, so we can instantaneously send updates to the app rather than requiring multiple updates for users. With the installation of Firebase and its respective Cocoapods, then I could begin coding.

Since Swift is designed as an object-oriented language, nearly every screen of the WECode app has a respective code file that connects the actions and outlets of the screen to the code. Therefore, I made each view controller its own code file connected to the elements on the respective screens. I then built the app on a page-by-page basis. I began with implementing the user authentication, then I worked on the Profile page and its components, as they all handled the personal information of the user. Then, I moved onto the broader elements of the app like the For You & Schedule pages, as they handled information that was separate from the user. These pages instead handle Firebase data directly from the WECode team, which is loaded separately from the application. The WECode team can simply upload our schedule and have it organized automatically in Firebase, making it incredibly dynamic, which is why I chose to use Firebase for this project. Finally, I delved into the Interact page, which was a bit more complicated as it combined all of the users information and allows users to write to the database directly. I addressed this last, as it required elements of all previous pages. I will go into more technical detail in the next section regarding the basic structure of my interactions with my code and the database.

Outside of the view controller files, I also organized my project into main folders: view controllers, custom views, and models. The CustomViews tie the custom-made cells with its respective table view, which I will discuss in-depth in the Interact section. For now, an example would be that I designed the schedule of events to show the locations, titles, times, and descriptions of each event using custom classes in CustomViews, which helped simplify my storing of information in the app and database. The code in CustomViews and Models are classes that can be utilized within the overarching view controller files, and they were incredibly helpful. I created the files in Models for pieces of information that I could benefit from by grouping them together. For example, I created an Event class, an Interaction class, a Comment class, and more, as I could create arrays of these custom classes in which to store the JSON from Firebase. The combination of my ViewControllers, CustomViews, and Models comprised the magic behind the app. 

Now, I will talk a bit about the code behind each main section.

## Design of 4 Main Pages: For You Page

Since the For You page is not currently very exciting, as the conference has no current announcements. I will use this section to discuss the overall breakdown of Swift code files. View controllers are arranged in files with classes, where the initializer is considered the viewDidLoad() function, as it loads the page for the user. Any global variables and outlets are typically included above the viewDidLoad() function, as it is a common stylistic practice. Thus, any actionable functions, like retrieving data from Firebase or calling a function when a button is clicked, is handled below the viewDidLoad() function.

## Design of 4 Main Pages: Interact Page

In the Interact page, I performed the typical class set-ups and initialized my actions and outlets. Then, I set up the tableView delegate and data source, as well as their essential functions needed in order to load data into the tables. I utilized a custom-made InteractTableViewCell class and custom Interaction class to help organize my data, as the Interact page would contain messages from users. Utilizing the custom cell would allow me to have more control over the appearance and organization of the data, so instead of directly loading the Firebase data about interactions between users into the table (which would involve very repetitive, messy code), I loaded my data from the database as an array of custom Interactions, then used the custom cell to automatically load them onto the user's screen. Besides this initial complexity, the trickiest part of the Interact page was viewing the information from the database, so I made this its own function that sorts out each type of interaction (Q&A vs. Resource). Then, I parsed through the database JSON with loops and utilised my custom classes.

## Design of 4 Main Pages: Schedule Page

The implementation of the Schedule page was very similar to the Interact page. It essentially configured the actions, outlets, and global variables, then loaded the schedule data from Firebase into a custom-made table. This time, I created a custom-model Event and custom-cell ScheduleTableViewCell to organize my information, and I utilized the same breakdown as the previous section to take the scheduling data from Firebase and present it to the user. 

## Design of 4 Main Pages: Profile Page

Lastly, the profile page was a bit more challenging to set up in regards to connecting actions, outlets, and global variables, except its functions were rather simple. After loading the initial view controller, I used the function retrieveData() - which is also present in all other pages - to load the user's data onto the screen directly. Then, I implemented the QR code buttons to take the link of the user's social/linkedin and pass it to the next page, or I directed the user to update their information. This page was rather simple in terms of code, and I could re-use the retrieveData() function in following pages, as it established how to view data from pathways in the Firebase database!

## Final Thoughts

All in all, when coding this project, utilizing classes and objects were my closest friendships, as they greatly simplified the organization of my data. Additionally, understanding how to navigate database pathways in Firebase was also critical to obtaining the correct information in the correct places!

Looking back, I believe that approaching my application with the user's experience first-and-foremost in mind both assisted the way I designed the app, as well as how I coded the app more intuitively! From using QR code libraries for the first-time, to understanding the complexity of storing images in a database, this project was both incredibly helpful for my coding abilities and for my organization! I am excited to continue growing the platform, refining it, and using it at the conference in February!

Please let me know if you have any questions/feedback!

## Thank you! Happy coding!