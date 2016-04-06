# Webby bot template

Clone the code, run webby demo bot with commands

```shell
$ git clone https://github.com/gasolin/webby-template.git demo
$ cd demo
$ npm install
$ ./bin/webby
```

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
```

### Facebook Messenger
Support via [hubot-messenger](https://github.com/kimberli/hubot-messenger)

```
npm install hubot-messenger
```

Edit `src/messenger.coffee` and replace `hubot` to `webbybot`.

Add related parameters in `.env`:
```
export HUBOT_FB_USERNAME=
export HUBOT_FB_PASSWORD=
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
```
