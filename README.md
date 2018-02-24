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
2. Create schema for storing messsages in a database
3. Create SQL scripts for adding, finding and deleting
4. Implement back end API for sending messages
5. Create a message class to store message information
6. Give the user a notification if they have a new message
This user story and the next user story were initially how they are now. One day I was absent and the team decided to merge them together into the same user story, which is understandable. I was under the assumption that only one person can work on a user story at a time, because that is how it is normally done at my work. However, I have now realized that any number of people can work on a user story and different developers can be assigned the tasks of one user story. In retrospective I think that having this as one user story may be better, and I think it caused some confusion in the group when I split it back into two separate stories as it was originally.
I assigned this story a priority of 10 because it is pertinent to the functionality of the app and the app cannot be created without it. I estimate that it will take about 10 days to finish this user story. Alot of the time will be spent on the user interface, and some time will also be spent creating the back end. The SQL should only take about 1/2 a day.

# Send Messages
### User should be able to send messages to matches
#### Priority: 10
#### Estimate: 10
1. Create REST service to send messages and the required SQL
2. Create view to send messages
This is one of the user stories that contains the tasks that I wrote. In hindsight maybe I should have broke the first task into two separate tasks but cards were relatively short. I think it is rather shorter and simpler than the Recieve messages one which I did not do but the student said is from the book. I was suprised at how well that one was done. This one however embodies the two most main important tasks of the user story. This user story should take the same amount of time as the Recieve messages story and it has the same priority for the same reasons. It would also make sense to have the same developer do these two stories because they will become familiar with the similar back-end services as they will probably use the same controller.

# View Test Results
### The user will be able to view their test results at will
#### Priority: 15
#### Estimate: 12
1. Create SQL table to store results
2. Create view to display test results
This user story is linked to the Take Personality Test user story, and maybe it would make sense to have the same developer do these two stories. This story is also a very simple one. The task for the first one kind of overlaps with the first story and it should maybe be like "create the business logic to retrieve the stored results" which probably will require creating an API which will accept a GET request. I assigned it an estimate value of 12, as I find that POST requests are a little harder to do than GET requests, and by going off the similar story having 10, a value of 12 seems appropriate. The priority is 15 because it is not necessary for the application to function correctly it is just of huge convenience to the user to be able to see their test results.

# Set User Age Preference
### User decides the parameter for what age range they want
###  their matches
1. Create user interface / integer slider to create an age range<br /> preference

# Accept / Decline Matches
### The user will be able to accept or decline matches in a list,<br /> removing them from a potential match to be accepted or <br /> declined
1. Create UI for matching with accept / decline (Picture)
2. Create schema & scripts for DB storing who the user accepts<br /> / declines
3. Notify user if they have a successful match
4. User personality data to predict the best match

# Create Type Preferences
### The user will be able to alter what type of personality<br /> they prefer to match with. The preferences will default<br /> to what researchers believe is the 'perfect' match for <br /> your type.

# Set User Gender Preference
### A user will set their gender preference for matches. Will be<br /> opposite sex by default.

# See Photos After Match
### The user will be able to view photos of their match only<br /> after both people have accepted each other as a match

# Change Application Notification Settings
### When another match sends a message or other reason for a<br /> notification be able to turn off/on
