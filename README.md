The Checklist
You can read the full checklist in CHECKLIST.md.
To view/edit the raw data, see personal-security-checklist.yml

The Website
The easiest method for consuming the checklist is via our website, at: digital-defense.io

Here you can browse lists, filter by your threat model and tick items off once complete (plus, there are pretty charts to make you feel good about your progress ☺️).



About
The source for the website is in web/.
The site is built with Qwik, using TypeScript and some components from DaisyUI.

Developing
To run the app locally, or to make code changes, you'll need Node and Git installed.

Grab the code: git@github.com:Lissy93/personal-security-checklist.git
Navigate into source: cd personal-security-checklist/web
Install dependencies: yarn
Start the development server: yarn dev
Alternatively, just open this repo in Code Spaces, where everything is already configured and ready to go.

Deploying
To deploy the app, follow the developing steps above, then run yarn build,yarn build.static. You can then deploy it by copying the dist/ directory to any CDN, web server or static hosting provider of your choice.

Alternatively, fork the repo and import into your providers dashboard. Or use the link below for an easy 1-click deploy 😉

The API
We also make all the data available via a free API, which you can use however you wish.

Usage
All endpoints are documented in our OpenAPI spec, you can view these and try them out via our Swagger docs.

Base: digital-defense.io/api

/api/checklists /api/checklists/[name-or-index] /api/checklists/[name]/[point-index] /api/search/[searchterm]

Developing
Deploying
Contributing
All checklist data is stored in personal-security-checklist.yml. This is pulled in the website at build-time, and referenced by the API, and is also dynamically inserted into the markdown Checklist page.

So if you only wish to make changes to the data, this is the only file you need to edit.

Important: When submitting your pull request, provide references backing up any information that you're adding/amending/removing.

For modifying the website or API source, see the developing sections above for instructions on running locally.

Prior to submitting an issue or PR, please ensure you've followed the community guidelines and followed the Code of Conduct.

