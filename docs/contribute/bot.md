# Contribute to the bot itself
## Getting started
1) In oder to start programming and contributing you need to clone the repository of the bot.

```
# Using ssh
git clone git@github.com:Azorimor/azolyzer.git

# Using https
git clone https://github.com/Azorimor/azolyzer.git
```

2) Open the folder you just cloned with your favorite Terminal and install the dependencies.

```
# For the backend
cd backend
npm install

# For the frontend (Web interface)
cd angular-frontend 
npm install
```

3) Open the folder in an editor. Now copy the file named **.env.example** and name the copied file **.env**.  
Now you need to change some values here. Currently only the value for the **DISCORD_TOKEN** needs to be set.  
Navigate to the discord developer portal and register an application. Then you can change your application to a bot application and copy the token of the bot into this **.env** file.

4) Now you need to setup the database for development. This is currently done by using the default *docker-compose.yml* file. You need to have docker and docker-compose installed on your machine.

```
# Inside the backend folder run
docker-compose up -d
```

5) Now the bot can be started for development by running the following commands.

```
# For the backend in the backend folder
npm run start:watch

# For the frontend in the angular-frontend folder
ng serve
```

6) If you want you probably should install the angular-cli globally aswell, if you are working on the frontend. 
If your working on the backend and want to make changes to the database it is also recommended to install the typeorm-cli globally.
Visit the official documentations for further informations.