#  Take Personality Test
### User takes personality test (redirect to site).
#### Estimate: 5
1. Find suitable Myers-Briggs personality test to link to
2. Add link to take personality test to views

# View Matched Users
### The user will be able to view previous matches
#### Estimate: 8
1. Create user interface that shows all previous matches
2. Create schema for database that stores all successful matches
3. Create SQL script for adding all past matches into database
4. Link each match to an on-going or possible conversation

# Edit Profile
### Change what other users see on their profile; such as a bio<br /> and details
#### Estimate: 5
1. Create user interface with editable text boxes that correspond<br /> to the data on the user's profile
2. Create SQL database holding the data of the user's profile.<br /> Also include scripts to change/get database info.

# Set Preferred Distance of Matches
### The user will be able to choose a preferred location (or <br /> distance away) for their matches.
#### Estimate: 3
1. Add preferred distance column to user settings table
2. Add preferred distance to user settings page (view)

# Recieve Messages
### A user will view an inbox of all incoming messages
1. Create user interface for incoming messages
2. Create schema for storing messsages in a database
3. Create SQL scripts for adding, finding and deleting
4. Implement back end API for sending messages
5. Create a message class to store message information
6. Give the user a notification if they have a new message

# Send Messages
### User should be able to send messages to matches
1. Create REST service to send messages and the required SQL
2. Create view to send messages

# View Test Results
### The user will be able to view their test results at will
1. Create SQL table to store results
2. Create view to display test results

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
