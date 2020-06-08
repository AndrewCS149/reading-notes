# Intro to Heroku with Node.js

---

### Create an app via the command line

Step 1: Create repo on github

Step 2: Clone repo to local machine

`$ git clone [link from github]`

Step 3: Create heroku app command: 

`$ heroku create [app-name]`

Step 4: Deploy code

`$ git push heroku master`

Step 5: Open the deployed app to see if it deployed correctly

`$ heroku open`

---

### View Activity logs via the command line

`$ heroku logs --tail`

---

### Locally run your app

`$ heroku local web`

---

### Push local changes

1. `$ git add .`
2. `$ git commit -m"Message"`
3. `$ git push heroku master`
4. `$ heroku open [app name]` (open the app to check if changes went through)

--- 



