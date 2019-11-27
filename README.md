# cloud-functions-typescript-boilerplate

boilerplate for development Google cloud functions by TypeScript

# npm scripts

```sh
$ npm run http:start
```

Start http function on your local PC. After this command you can access via `http://localhost:8080`.

```sh
$ npm run event:start
```

Start Pub/Sub backend function on your local PC.

```sh
$ npm run event:local-publish
```

After above command you can publish pubsub message to you local function via `curl` and POST `scripts/event/local-data.json`.

```sh
$ npm run http:deploy
```

Deploy your http function to Google Cloud Functions as HTTP trigger function.

```sh
$ npm run event:deploy
```

Deploy your Pub/Sub background function to Google Cloud Functions as Pub/Sub trigger function. If you want to change topic name, please rename topic name on `scripts/evenet/deploy.sh`.
