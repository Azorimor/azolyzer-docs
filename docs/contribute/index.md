# How to contribute to the project
## Contribute to the bot itself
## Contribute to this documentation
This documentation is build by using [mkdocs.org](https://www.mkdocs.org). Visit the official site for their documentation.
On top of that, a [material theme](https://squidfunk.github.io/mkdocs-material/) is used.

### How to get started 
1) Clone Repository  

First clone the [repository](https://github.com/Azorimor/discordbot-docs) for the documentation.

    # Using ssh
    git clone git@github.com:Azorimor/discordbot-docs.git

    # Using https
    git clone https://github.com/Azorimor/discordbot-docs.git
  

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
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

### Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.