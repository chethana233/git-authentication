## Functionalities
- This website allows anyone to authorize their github account and create a sample repo with a dummy file in that repo. 
- Users can also delete a repo by this website.

The project is hosted on railway.app. Please click [here](https://web-production-86b3.up.railway.app/)
## How to run the project :-

```bash
$ npm install
$ npm link hbs
$ npm run start

Additonally create a new O Auth app on Github. Modify the Homepage URL and Authorization callback URL as required

add in the environment variables in the .env file in the following format 
CLIENT_ID=*****
CLIENT_SECRET=*****
OWNER_USERNAME=*****
OWNER_EMAIL=****

(if this is to be made to run locally we will also have to change the urls in the views accordingly as well)
eg: link.href = `https://web-production-86b3.up.railway.app/home?username=${username}`;
would change to 
link.href = `http://localhost:5008/home?username=${username}`
additionally the ports can be changed in the main.js
