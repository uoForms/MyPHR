# MyPHR Portal

<strong>Author: Wenyan Li</strong> <br>
(The repository is duplicated from my private MyPHR_Portal repository)

[MyPHR Portal](https://myphr-portal.firebaseapp.com/) is a patient endpoint of a patient-centric health data sharing system can be built using React and emerging support tools such as Google Sign-In and Google Places. The endpoint allows patients to view their health profile, activities and episodes, configure alerts as well as add/edit information. The CRUD operations are supported by a Python Flask API called MyPHR API.

The application is running on Firebase, you can access from the link: https://myphr-portal.firebaseapp.com/. <br>

## Login Page 

The account can be used to login: <br>
username: H7777666699  
password:mypass

Google OAuth is implemented with button "Login with Google", the account information can be retrieved after signing in with the correct credentials. Afterward steps about creating a new user in db is not implemented yet on api side.  

## Dashboard Page

The page is supposed to show some graphical representation of the patient's health activity data. It is hard coded now because there is no endpoint for it on api side.

## Profile Page

In Basic Info, Patients are allowed to modify their service language by choosing English or French.
In Health Profile, Patients are allowed to add more Dietary Regimen or Advance Directives by choosing from the option lists.
Patients can also update their contact information/caregivers' contact information. Every Save action needs checking which input value is updated and calling the specific api method. The address autocomplete is disabled for now because of a Google Places API Billing issue. Patients are not able to edit Physicians subpage.

## Alerts

Since there is no corresponding endpoint for alerts currently on api side. The text of the page is hard coded, and the date are called from a mock api. 


The project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Run

In the project directory, use:

### `npm start`

The application will run on [http://localhost:3000](http://localhost:3000).

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm run build`

Use the above command to build the application, and then the app will be ready to be deployed.


