# How to contribute to the project
## Contribute to the bot itself
### Getting started
1) In oder to start programming and contributing you need to clone the repository of the bot.

```
# Using ssh
git clone git@github.com:Azorimor/discordbot.git

# Using https
git clone https://github.com/Azorimor/discordbot.git
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

## Contribute to this documentation
This documentation is build by using [mkdocs.org](https://www.mkdocs.org). Visit the official site for their documentation.
On top of that, a [material theme](https://squidfunk.github.io/mkdocs-material/) is used.

### How to get started 
1) Clone Repository  

First clone the [repository](https://github.com/Azorimor/discordbot-docs) for the documentation.

```
# Using ssh
git clone git@github.com:Azorimor/discordbot-docs.git

# Using https
git clone https://github.com/Azorimor/discordbot-docs.git
```

2) Install mkdocs and the material theme.  

As mentioned above, visit the [official documentation](https://www.mkdocs.org/#installation) for more detail.
You need to make sure, Python 3.x and pip is installed on your computer. Not every Python version is supported today.
Now you can install mkdocs and the material theme. 

```
pip install mkdocs
```

```
pip install mkdocs-material
```

For more information about the used material theme, visit the [documentation](https://squidfunk.github.io/mkdocs-material/getting-started/).

### Commands

* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs -h` - Print help message and exit.

### Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.