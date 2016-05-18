# Webby bot template

[Webbybot](https://github.com/gasolin/webbybot/) is the next generation message/chat bot framework written in ES6 and plain javascript. Fully compatible with [Hubot](https://github.com/github/hubot)'s middleware and plugins.

Clone the code, set webby bot with commands

```shell
$ git clone https://github.com/gasolin/webby-template.git demo
$ cd demo
$ npm install
$ ./bin/webby
```

You can run your bot with new webbybot core `./bin/webby` or test plugins with hubot core `./bin/hubot`.

You can find and install extra skills from [npm](https://www.npmjs.com/search?q=hubot)

Enable a skill in `external-scripts.json`.

You can add the environment variables in `.env` file or defined in system PATH.

## Workable adapters

We've successfully run webbybot with Telegram, Facebook messenger, Skype adapters. You are able to try with other adapters via [instruction](https://github.com/gasolin/webbybot#how-to-replace-hubot-to-webbybot).

### Telegram
Support via [hubot-telegram](https://github.com/lukefx/hubot-telegram)

```
npm install hubot-telegram
```

Edit `src/telegram.coffee` and replace `hubot` to `webbybot`.

Add related parameters in `.env`:
```
TELEGRAM_TOKEN=
WEBBY_CURRENT_ADAPTER="telegram"
```

Run bot with telegram adapter
```
./bin/webby -a telegram
```

### Facebook Messenger
Support via [hubot-messenger](https://github.com/kimberli/hubot-messenger)

```
npm install hubot-messenger
```

Edit `src/messenger.coffee` and replace `hubot` to `webbybot`.

Add related parameters in `.env`:
```
HUBOT_FB_USERNAME=
HUBOT_FB_PASSWORD=
WEBBY_CURRENT_ADAPTER="messenger"
```

Run bot with messenger adapter
```
./bin/webby -a messenger
```

### Skype
Support via [hubot-skyweb](https://github.com/EllisV/hubot-skyweb)

```
npm install hubot-skyweb
```

Edit `src/skyweb.coffee` and replace `hubot` to `webbybot`.

Add related parameters in `.env`:
```
HUBOT_SKYPE_USERNAME=
HUBOT_SKYPE_PASSWORD=
WEBBY_CURRENT_ADAPTER="skyweb"
```

Run bot with skype adapter
```
./bin/webby -a skyweb
```
