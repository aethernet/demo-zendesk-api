Very crude / basic PoC of a support portal using zendesk api

This validate : 
  - [x] creating tickets using Zendesk api and a custom form
  - [x] retrieving tickets for a user

Next thing to test would be:
  - [ ] retrieve / show threads for tickets
  - [ ] research how to properly authenticate user


How to use : 
  - use a test account valid for premium.balena.io (i.e. create a new user account from agent dashboard)
  - create a password for the account (from the account creation confirmation email)
  - use email and password on the form and submit or retrieve tickets

Read the code : 
  - everything useful is in src/pages/index.tsx

Develop :
start a nextjs develpment server
  - clone
  - npm i
  - npm run dev

Build :
build a static site in `out` folder
  - clone 
  - npm i
  - npm run build

Deploy :
build a docker container with a simple http server to serve the static files
  - build (see previous point)
  - balena push **fleet**
  - turn on "public url" for a device