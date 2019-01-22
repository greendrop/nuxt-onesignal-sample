# nuxt-onesignal-sample

# aed-map

OneSignalとNuxt.jsを使用したPush通知サンプルです。

## 使用言語・ライブラリ

- OneSignal
- Nuxt.js(Vue.js)
- Vuetify

## 環境構築アプリケーション

- Docker
- Docker Compose
- direnv
- git

## セットアップ

```shell
$ git clone git@github.com:greendrop/nuxt-onesignal-sample.git
$ cd nuxt-onesignal-sample
$ vi .envrc
$ direnv allow
$ cp .env.example .env
$ docker-compose pull
$ docker-compose build
$ docker-compose run --rm front bash
$ yarn install
$ exit
$ docker-compose up
```

### .envrc

```
export USER_ID=`id -u`
export GROUP_ID=`id -g`
```

### .env

OneSignalのApp ID

```
ONESIGNAL_APP_ID=XXXXXX
```

## ブラウザで表示

http://localhost:3000
