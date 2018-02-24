### Nicholas Gallimore (nfg3@zips.uakron.edu) - Team Jar Jar Binks
# Myers-Briggs Personality Test Dating App
#### This is a report on the development process of the user stories for a Myers-Briggs Personality test dating app that uses your personality type to find your "perfect" match. This application will have the user take the Myers-Briggs Personality Test to find what their unique personality will be when they sign up. This will then be used to find people that are considered a match based on the user's personality. User stories will be listed, following which their estimate (in days) and their priority ranking (lower number means higher priority), and an excerpt explaining a detailed process as to why these values were chosen and maybe changes to be considered. These user stories are not perfect but due to extenuating circumstances they must be used. All of the user stories that had incomplete tasks, estimates and priorities, I filled in. However if something was decided amongst the team, then that is what is written. If I disagree with said decision or have comments on how to change the user story, tasks, priority, or estimates, it will be mentioned in the explanation. I will also try to comment on the processes that were used to come up with each user story, as well as the general overall process at the end. Hopefully in doing this report, this process of creating user stories will become more clear and efficient for me, because I realize that such a process like this ***can continuously be improved***.

#  Take Personality Test
### User takes personality test (redirect to site).
#### Estimate: 5
#### Priority: 10
1. Find suitable Myers-Briggs personality test to link to
2. Add link to take personality test to views
3. Store personality test results in database
***
We figured that this could be implemented using a browser within the app. The personality test one of the group members was talking about using (I do not have the link) had the results in the URL and we would be able to parse the URL for the results.
The reason for choosing five days is because it could take longer than expected, however it should not take too long. It is a fairly easy user story. I assigned this a priority of 10 because the application would not adhere to the original design idea of the application, and would too closely resemble Tinder without this. This is what separates the app from the competition and without it the application is a regurgitated idea. This user story might be implemented using a back end API service with a POST request.

# View Matched Users
### The user will be able to view previous matches
#### Estimate: 8
#### Priority: 10
1. Create user interface that shows all previous matches
2. Create schema for database that stores all successful matches
3. Create SQL script for adding all past matches into database
4. Link each match to an on-going or possible conversation
***
The story is intended to make it so that users will be able to see their previous matches. The most complicated and longest task on here is creating the user interface. There will be lots of design and user experience decisions involved in this. There will be a fair amount of business logic involved too which may take a couple days. Even though the team (two of us) decided to choose 8 days for this, in retrospective I would assign it more like 15 days. I assigned it a priority of 10 because the app would not be usable without this feature. It is pertient and is part of the main functionality of the application.

# Edit Profile
### Change what other users see on their profile; such as a bio<br /> and details
#### Estimate: 5
#### Priority: 20
1. Create user interface with editable text boxes that correspond<br /> to the data on the user's profile
2. Create SQL database holding the data of the user's profile.<br /> Also include scripts to change/get database info.
***
This is a feature that is not as pertinent to the application but is still pretty essential. This gives the user a chance to stand out amongst the crowd and enter customized text into their profile, which will probably give other users a better idea of the personality of the user than just the personality test matching algorithm alone. I assigned this a priority of 20 for this reason, as the app can be implemented without this feature, and there are alot of other things that are required for the application to become fully functional, which should be the goal for the first iteration. The reason this user story has only five days is because it is just simply creating the view to display content that is stored in the database. In retrospective thinking back to it, it may be assumed that the profile page is already created and we may have to create the routing for the actual page and create the actual profile for each user first before we can implement this, so maybe it will take a little bit longer than five days if the profile is not created. Better yet I would change this story to "Create user profiles"

# Set Preferred Distance of Matches
### The user will be able to choose a preferred location (or <br /> distance away) for their matches.
#### Estimate: 3
#### Priority: 15
1. Add preferred distance column to user settings table
2. Add preferred distance to user settings page (view)
***
This user story also has a major underlying assumption that there is a settings page, which in the case that it already exists -- sure it would only take at most three days (to set the preferred distance as a column in a database table) but to actually implement the intended functionality of what this story should actually be, might take a little bit longer as it would have to implement geolocation services and given my experience with that (none) I would increase the estimate to maybe 10 days. If there is no settings page, then it will be required to make that as well. Which should increase it by maybe an extra 3 days as it would only be a relatively simple view that only gets and sets data in the database. I would not change the name of this but maybe I would add a task such as "create configuration page". This has a priority of 15 because it is not quintessential to the functionality of the application but it is still relatively important. Ideally the point of the application is to meet people to go on dates, and you cannot exactly do that if they live very far away. This definitely should be in the first iteration though.

# Recieve Messages
### A user will view an inbox of all incoming messages
#### Priority: 10
#### Estimate: 10
1. Create user interface for incoming messages
2. Create schema for storing messages in a database
3. Create SQL scripts for adding, finding and deleting
4. Implement back end API for sending messages
5. Create a message class to store message information
6. Give the user a notification if they have a new message
***
This user story and the next user story were initially how they are now. One day I was absent and the team decided to merge them together into the same user story, which is understandable. I was under the assumption that only one person can work on a user story at a time, because that is how it is normally done at my work. However, I have now realized that any number of people can work on a user story and different developers can be assigned the tasks of one user story. In retrospective I think that having this as one user story may be better, and I think it caused some confusion in the group when I split it back into two separate stories as it was originally.
I assigned this story a priority of 10 because it is pertinent to the functionality of the app and the app cannot be created without it. I estimate that it will take about 10 days to finish this user story. Alot of the time will be spent on the user interface, and some time will also be spent creating the back end. The SQL should only take about 1/2 a day.

# Send Messages
### User should be able to send messages to matches
#### Priority: 10
#### Estimate: 10
1. Create REST service to send messages and the required SQL
2. Create view to send messages
***
This is one of the user stories that contains the tasks that I wrote. In hindsight maybe I should have broke the first task into two separate tasks but cards were relatively short. I think it is rather shorter and simpler than the Recieve messages one which I did not do but the student said is from the book. I was suprised at how well that one was done. This one however embodies the two most main important tasks of the user story. This user story should take the same amount of time as the Recieve messages story and it has the same priority for the same reasons. It would also make sense to have the same developer do these two stories because they will become familiar with the similar back-end services as they will probably use the same controller.

# View Test Results
### The user will be able to view their test results at will
#### Priority: 15
#### Estimate: 12
1. Create SQL table to store results
2. Create view to display test results
***
This user story is linked to the Take Personality Test user story, and maybe it would make sense to have the same developer do these two stories. This story is also a very simple one. The task for the first one kind of overlaps with the first story and it should maybe be like "create the business logic to retrieve the stored results" which probably will require creating an API which will accept a GET request. I assigned it an estimate value of 12, as I find that POST requests are a little harder to do than GET requests, and by going off the similar story having 10, a value of 12 seems appropriate. The priority is 15 because it is not necessary for the application to function correctly it is just of huge convenience to the user to be able to see their test results.

# Set User Age Preference
### User decides the parameter for what age range they want <br />their matches
#### Priority: 15
#### Estimation: 10
1. Create user interface / integer slider to create an age range<br /> preference
2. Create API to store the information
***
This user story is also under the assumption that there is a configuration page. So if one of other configuration stories were done first than this would take shorter. Given that I gave the priority for this a priority of 15 either one could be done first (referring to the edit profile user story). This estimation however is assigned under the assumption that this story is the story to first create the interface for the settings page. I assigned the estimation a value of 10 given the circumstances of creating the routes and the initial part of the view. The priority was given a value of fifteen because it is kind of important for the user to have relevant matches or they will not like it, but it is still possible to use the application without this feature. It would be fundamental and essential to a full fledged version of this application and that is why I would recommend to ship this feature out in the first iteration.

# Accept / Decline Matches
### The user will be able to accept or decline matches in a list,<br /> removing them from a potential match to be accepted or <br /> declined
#### Priority: 10
#### Estimation: 20
1. Create UI for matching with accept / decline (Picture)
2. Create schema & scripts for DB storing who the user accepts<br /> / declines
3. Notify user if they have a successful match
4. User personality data to predict the best match
***
This user story is part of the core functionality of the application. In fact this is where we as a team decided to put the matching algorithm, and it is very important indeed. After reviewing this when we went to do the estimation I wanted to put the algorithm task into a separate story but that did not happen due to time constraints. I feel that this story has enough on its own in UI and business logic to take 15 days even without the matching algorithm. There will have to be AI built into the algorithm if it is to be anything comparable to the other services that are currently out there, and I think that is out of the scope of any of us and would require some pretty heavy research and as I am told, lots of math. I gave this user story a priority of 10 because it is pertinent to the functionality of the application and the application would not be usable without it. I also would maybe put the notify user if they have a successful match into a separate user story too. I gave this story an estimation of 20 because we should go back and try to reduce the number of tasks tagged onto this story, as it is already very large. I am not able to speak on the process for creating these tasks as I did not create them.

# Create Type Preferences
### The user will be able to alter what type of personality<br /> they prefer to match with. The preferences will default<br /> to what researchers believe is the 'perfect' match for <br /> your type.
#### Priority: 20
#### Estimation: 8
1. Do UI changes to settings page
2. Perform SQL changes
3. Create POST and GET methods on controller for API
4. Tie data into matching algorithm (e.g., with if statements)
***
This is a cool feature that allows the user to take control of their matching algorithm if they want to do it purely on what personality type the user thinks they like. This is closely related to the Accept / Decline matches story and maybe should be done by the same developer. It will have to be tied in with the matching algorithm logic when retrieving a list of potential matches for the user to swipe through. I gave this a priority of 20 because it is not pertinent to the functionality of the app. It a value of 8 for the estimation because it should not take too long, the longest part probably will be doing both of the back end API changes. The UI change is relatively minor. Tying the data into the matching algorithm should not be too hard either. If it is simply a filter to only select users with the personality type that the user chose, then it is very simple.

# Set User Gender Preference
### A user will set their gender preference for matches. Will be<br /> opposite sex by default.
#### Priority: 10
#### Estimation: 8
1. Do UI changes
2. Perform SQL changes
3. Create POST and GET methods on controller for API
***
This user story is pertinent to the app. It is becoming more and more common for people to have different sexual orientations, as well as transgender etc. Technically we should have a box for "other" if we want to be culturally sound. This user story should be pretty basic though. It shouldn't require much time, some basic UI changes that will be added to the settings view that was created in the set user age preference story. The SQL is also very basic and should not take very long. Overall I would say that this should take no longer than 8 days if you are slow at doing the backend side of things. This obviously has a priority of 10 because we do not know what gender the user prefers and the app would not be usable without it.

# See Photos After Match
### The user will be able to view photos of their match only<br /> after both people have accepted each other as a match
#### Priority: 10
#### Estimation: 15
1. Add the UI changes to view the picture on the profile page of the accepted matched user
2. Create a file system to store the photos
3. Create a POST and GET request to retrieve the photos\
4. Modify the configuration settings page to upload a photo for the user
***
I absolutely did not see this user story before and I have to say that I am not sold on the idea of not showing the pictures of people before they are matched. We should show them the pictures before the match. But if we were required to implement this story then it would probably not be very fun. I am working on creating a media library for the press to download images from, and have say that a senior developer spent a year on the project and I just had to spend 12 days doing styling changes. While this is not anywhere near the scope of that, I feel that dealing with photos might prove to be a challenge. Where do you store them? Do we have to set up a CDN? If so then this story is completely longer than 15 days. If it is just stored in a file system on one server then sure maybe it can take 15 days. I gave this story a priority of 10 because far less people will still want to use the application if they cannot see pictures of the people they are potentially going on a date with, unless you market it as some form of a blind-date app, but that's just cheap. We must also assume that there is an upload photo feature too on the edit profile page.

# Change Application Notification Settings
### When another match sends a message or other reason for a<br /> notification be able to turn off/on
1. Create toggle on the settings view
2. Create SQL table and add foreign keys
3. Create POST and GET requests on the controller for the API
***
#### Priority: 20
#### Estimation: 5
This is relatively simple feature and I think it may even be required to be integrated with iOS. If it is required then of course the priority would shift to 10. This should not take very long. The SQL to create is very simple. We came up with this story because we decided to make individual user stories for each settings, something which I think is valuable because it allows to choose which configuration settings we want to have first and we can go back and do the other ones later that have a lower-priority. This is helpful if there is a deadline that is approaching and we need to cut back on some user stories. This is definitely one of the ones that may be possible to cut out if it is not necessary to have. This probably should be in a second iteration of the application. The user does not need to control when they are notified to use the app, so that is why it has a priority of 20. The five days I think is fair based on the given tasks.

# Overall
Overall, I think the project was a success. I have learned how to manage user stories better and have improved on the process used to create them. I think the process of creating the user story first, going back and revising, then adding tasks, then doing an estimation is a good workflow and is something that I will start to do. The only thing that I wish we could do is maybe add tasks for testing. As that is a very important element of the software development process and it should probably be recorded who did the testing. Test cases should be assigned after writing the tasks as well. I know I was not able to comment on the individual process specifically of each user story but I did my best to encapsulate my thoughts when they were being created and how I would go about implementing them. Thinking about the actual process of creating user stories and trying to improve upon it is something that is hard to do, I have learned.
