# fullstack

## Project setup
```
yarn install

yarn serve        // Compiles and hot-reloads for development
yarn build        // Compiles and minifies for production
yarn lint         // Lints and fixes files
yarn test         // Run your tests
yarn test:watch
```

## Log

* Created `docker-vue-test` app on EB, with an env called `docker-vue-test-env`.
* Setup travis.yml
* Pickup s3 bucket name (Travis will upload a zip of the app on a particular s3 bucket to be picked up by ElasticBeanstalk
* Get access keys for Travis-CI, in AWS Console, IAM
	* Generate new user for TravisCI
	* Attach existing policies => “Provide full access”
	* Copy acces-key and secret-key
* Add keys to travis-ci.org > settings > environnement variables
* Switched to instance `t2.micro` (might be because of `npm install` timing out).
* Deleted setup to not be billed. Might be restored for a bit.