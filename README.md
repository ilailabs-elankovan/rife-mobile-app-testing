### Rife Mobile App - Testing 

*This page is intended for the internal team at ilaiLabs, and should be reffered as instruction manual for testing Rife Mobile App.*

[Feature App - Demo Video]()

Devices: iPhone

**Feature list - Feature App**

1. Project Setup: Successfully established the project and environment, including GitLab repo,
GCP, Firebase Account, and Rowy admin dashboard. Admin can configure Master Sequences,
Player Settings from firebase.

3. Signup Module: Implemented the ability for mobile users to create a new account and
access the app. The user data is recorded in the backend including the app consent details
and issues selected during the signup process.

4. Social Media Login: Users can login or singup via social media - to access the application. 

5. Login Module: Enabled existing members to log in to the application and access its
features.

7. Social Media Login: Users can now sign up or log in using their Google or Facebook
accounts.

9. Reset Password: Implemented a feature allowing users to reset their passwords through an
email link.

11. Logout: Users can now properly log out of the application using the 'logout' button on the
app's home page.

13. Onboarding Screens: Implemented onboarding screens for first-time app installations.
Images and videos can be dynamically configured from the Rowy dashboard.

15. Home Screen: The home screen displays a video about Rife technology and includes a FAQ
section.

17. Configure FAQs: The admin can configure the FAQs, add or edit the title or text from the
backend.

19. Sequences Screen: Lists master frequencies, allowing users to click on a sequence and
navigate to the player to play the sequence.

21. Player Home: The player home includes a default frequency and duration for testing. Users
can play the sequence from the list in the Sequence Home or Playlist Home.

22. Play Sequence: The player can play frequencies in the given sequence. The user can click
play and stop the player.

24. Shop Menu: The app opens an in-app browser from the app to view the Rife Shopping
website.

------------------------------------------------

**Testing Instruction**

**APP HOME & BASICS**

**Onboarding Screens**
• Install the app for the first time, you can see the onboaridng screens. 
• Edit the content from the backend see if it gets dynamically updated in the app; //todo-elango; 

**Naviatation**
Assume the login is successful. 
• The app will display 5 pages to naviagate. Ensure you can navigate somoothly to all pages. 

**Logout**
• Click on the 'logout' button on the application home. It should logout and navigate to the login page. // BUG: Todo-elango; after logout; still naviagting to the app home;

**Login**
• If user is already sigined in - then he must be able to login; 
• If login credentials are wrong; this must be displayed in the tint message; 

**Social Media Login**
// TODO; TESTING TO BE DONE BY DEVELOPER; 

**Forget Password**
• Enter the email address, you will recieve the reset password url; click and reset password; try to login again; 

**Create User**
• Select the issues; app will allow if no issues are selected;
• Consent form; it should display the form; user should click on agree and enter name; if not this should not allow the user to next screen navigation. 
• Give all the credentials. Password must match; if all valid fields; account created. 

**Home Menu**
• Ensure 'favourite sequencies' section is displayed. If not 'no favouties sequences found message should be appearing' 
• Home page will have FAQ section; ensure this is displayed by default; You can expand and collapse. 
• If he/she is a first time user display the 'about_us video'. If user logged in the video should not appear. 

*Backend Testing(Elango, Raziqa)*
TODO; by Raziqa and Elango
• Update the FAQ title and body - see if this is reflected in the app. // to be done; 

*Favourite Seq Section*
• The sequences marked favourites in the SEQUENCE MENU should appear in the HOME PAGE. 
• The squences can be marked un-favourites and added or removed to playlist. 
• If un-favourite is done; on re-navigation to the page the updated list will appear; 
SUGGESTIONS FOR IMPROVEMENT: We can add refresh button in the app. 

**SEQUENCES HOME**
• Will display the list of sequences from the backend.
• Backend Testing: Update or modify the squences and see if this is populated in the app. // todo-elango-raizqa; 
• In the sequence card, you can *mark or unmark fav* and you can *add/remove* from playlist. 

**PLAYER HOME**
• Player home can be navigated form directly from bottom nav menu. Other way is to click on the *sequence card* from the *SEQUENCE MENU* OR *PLAYLIST MENU*
• When directly naviagted we have sample frequences. 
• When naviaged from squence card - the particular frequences are displayed in the player. 
• The user can click on the play button and stop button; 
• When the sequence is played it should move to other freq automatically. 
• The seq home should display the seq discription; 
• Ensure this is populated from backend; // todo-elango: Testing from backend. 

*BUGS* The freq card displays wrong duration in the app; it should display 3 instead of 30s; 

**PLAYLIST HOME**
• Only added seq must appear here.
• If removed it should not appear; // todo-elango: Fix the bug or add validations; 

**SHOP HOME**
• Should display the web-page browser; 

