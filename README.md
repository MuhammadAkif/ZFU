# Title

Keyflow-Event-Manager Standalone Server

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
```
Node
Npm
Dockers
```
### How to run and test keyflow-event-manager on your local machine
- Install node,npm and mamp.
- Clone keyflow-event-manager repository into your local machine.
- Run `npm install`, after that to auto update code changes to server you need to open a terminal in the project directory and run `make watch`.
- Now download MAMP and change document root for MAMP server.
- Steps to change document root for mamp server.
```
MAMP on MAC

1- Using Finder, select your HD device
2- Go to Applications > MAMP > conf > apache
3- Edit file  httpd.conf
4- Do a find on ‘DocumentRoot’
5- Replace the current path of your DocumentRoot (e.g.: /Applications/MAMP/htdocs) by your new (e.g.: /WebServers).
6- Do another find on ‘DocumentRoot’ until you get to the line that says “This should be changed to whatever you set DocumentRoot to.“
7- Replace the path on DocumentRoot (e.g.: /Applications/MAMP/htdocs) by your new path (e.g.: /WebServers).
8- Save the modified httpd.conf file
9- Go to MAMP
11- Select Stop Servers (if they are up and running)
12- Once the Apache and MySQL servers are stopped, select Start Servers
```
Now Open code in text editor or IDE Change the following files. (Note this will be improved in future version)

Uncomment beforeSend function from the following files.
- Event.js
- GuestsTable.js
- CardInfo.js
- VenueInfoController.js
- PaymentInfo.js

Update paths in url_helper.js file
- for api change path in base_api_path (Base path for api)
- for site_url change path in base_site_url (Base site url)

Update api_helper.js file
- Uncomment setAuthCookie() function.


Now open MAMP and click start server wait until apache server and MYSQL server are green.

You can check your site on this url:

http://stage-www.localhost:8888/mngr
