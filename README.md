dokku-bower-install
===================

Dokku pluging to install bower dependecies.

*NOTE*: it's developed and tested on latest `progrium/buildstep` which use latest `heroku-buildpack-nodejs`.

To install lastest build step, you should remove existing one and run,

```
$ docker build -t progrium/buildstep github.com/progrium/buildstep
```

## Description

This plugin will inject `/app/.bower` shell script, that's going to be executed on `pre-deploy` stage. If root of application contains `bower.json` file, then bower and all dependencies are installed.

## Usage

```
cd /var/lib/dokku/plugins
git clone https://github.com/alexanderbeletsky/dokku-bower-install
dokku plugins-install
```

Push you app.

# License

MIT
