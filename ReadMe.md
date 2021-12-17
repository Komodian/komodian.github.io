
### Prerequisites

- [Github Desktop](https://desktop.github.com/)
- [Hugo](https://gohugo.io/)
- Text Editor

### How to run this website on your local machine

You will need to install [Hugo](https://gohugo.io/) on your local machine to preview this website.

Follow "Install Hugo" instructions to install [hugo](https://gohugo.io/getting-started/installing/) on your machine.

### Clone website and edit contents

Follow this guide to clone this repo/website on your local machine:

https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop

Once you have this repository code on your local machine, you will be able to see a folder named "komodian-site-temp" at the location where you selected this rpeo to be cloned.

You can find content inside `komodian-site-temp/content/english/` directory.

Open the `.md` file in a text editor and edit the text following the markdown rules.

You can also read this [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to get up to speed what you can do to easily change the website pages with markdown format.

#### Preview the changes on local machine

You can preview the website using `hugo` command. Using command line terminal go to `komodian-site-temp/` directory and execute `hugo` command:

```bash
cd komodian-site-temp/
hugo server
```

You'll see some output like this

```bash
Start building sites …
hugo v0.90.1+extended darwin/arm64 BuildDate=unknown

                   | EN
-------------------+------
  Pages            |  55
  Paginator pages  |   1
  Non-page files   |   0
  Static files     |   1
  Processed images | 247
  Aliases          |   1
  Sitemaps         |   1
  Cleaned          |   0

Built in 315 ms
Watching for changes in /Users/satinder/Documents/GitHub/komodian-site-temp/{archetypes,assets,content,data,i18n,layouts,static,themes}
Watching for config changes in /Users/satinder/Documents/GitHub/komodian-site-temp/config.toml, /Users/satinder/Documents/GitHub/komodian-site-temp/config/_default, /Users/satinder/Documents/GitHub/komodian-site-temp/themes/bigspring/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/komodian-site-temp/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

If you see the output as shown above, open the URL http://localhost:1313/komodian-site-temp/ in your browser to view website.
Any changes you will save in your text editor will show automatically on this preview website if you keep running the `hugo server` command.

To exit or close the command `hugo server` press `CTRL+C` on your keyboard.

### Build website pages and push to github

Once you are done with your changes, generate website pages.

First go to the root directory of `komodian-site-temp/` and then execute the following commands:

```bash
cd komodian-site-temp/
hugo -d docs
```

This will generate/update `docs/` directory with HTML pages which you can now push to github. You can follow the guide from github docs to push the changes to github: https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/committing-and-reviewing-changes-to-your-project

