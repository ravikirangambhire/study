STEPS FOR DEPLOYING REACT BOILERPLATE ON HEROKU :::::

-->check the node and npm vesions and update in package.json file (engines)


MAIN STEP-1:
go to project folder in terminal and follow the following steps:::
--->heroku should be installed
--->heroku --version
--->heroku login --interactive    // logged in as ....
--->git init
--->git add .
--->git commit -m "First commit"
--->heroku create  // we get to links copy the second link
--->git remote add heroku https://git.heroku.com/murmuring-bastion-20818.git
---->git push heroku master
--->npm start (check whether it is working fine in local or not)


***FOR DEPLOYING REACT-BOILERPLATE EXTRA FOLLWOING STEPS TO BE FOLLOWED*****

MAIN STEP-2:(https://github.com/react-boilerplate/react-boilerplate/blob/master/docs/general/deployment.md)

STEP 1:SKIP
STEP 2:just follow what ever said in this step example---> """heroku buildpacks:set https://github.com/heroku/heroku-buildpack-nodejs#v134(must be given latest value) -a murmuring-bastion-20818(name you can get from heroku account)"""
STEP 3: (1)In package.json -->add "heroku-postbuild": "npm run build",  in scripts area (2) add  "prebuild": "npm run build:clean",  in scripts area
STEP 4: RUN the command "" heroku config:set NPM_CONFIG_PRODUCTION=false""
STEP 5:git add .
       git commit -m 'Made some epic changes as per usual'
       git push heroku master


*****AFTER YOU MAKE CHANGES IN YOUR LOCAL AND YOU WANT THE SAME CHANGES TO BE REFLECTED ON HEROKU THEN FOR RE-DEPLOYING PLEASE FOLLOW THE FOLLOWING STEPS***

STEP 1: git add .
STEP 2: git commit -m “any message goes here”
STEP 3: git push heroku master




