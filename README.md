<h1 align="center">
    <a href="https://electerm.github.io/electerm">
        <img src="https://github.com/electerm/electerm-resource/raw/master/static/images/electerm.png", alt="" />
    </a>
</h1>

# electerm

[![GitHub version](https://img.shields.io/github/release/electerm/electerm/all.svg)](https://github.com/electerm/electerm/releases)
[![Build Status](https://travis-ci.org/electerm/electerm.svg?branch=release)](https://travis-ci.org/electerm/electerm)
[![Build status](https://ci.appveyor.com/api/projects/status/33ckbqln02utekxd/branch/release?svg=true)](https://ci.appveyor.com/project/zxdong262/electerm/branch/release)
<span class="badge-daviddm"><a href="https://david-dm.org/electerm/electerm" title="View the status of this project's dependencies on DavidDM"><img src="https://img.shields.io/david/electerm/electerm.svg" alt="Dependency Status" /></a></span>
<span class="badge-daviddmdev"><a href="https://david-dm.org/electerm/electerm#info=devDependencies" title="View the status of this project's development dependencies on DavidDM"><img src="https://img.shields.io/david/dev/electerm/electerm.svg" alt="Dev Dependency Status" /></a></span>
<span class="badge-githubstar">
[![license](https://img.shields.io/github/license/electerm/electerm.svg)](https://github.com/electerm/electerm/blob/master/LICENSE)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

Terminal/ssh/sftp client(linux, mac, win) based on electron/ssh2/node-pty/xterm/antd/[subx](https://github.com/tylerlong/subx) and other libs.

<div align="center">
  <img src="https://github.com/electerm/electerm-resource/raw/master/static/images/electerm.gif", alt="" />
</div>

## Download/install

- [https://electerm.github.io/electerm](https://electerm.github.io/electerm)
- From release: [https://github.com/electerm/electerm/releases](https://github.com/electerm/electerm/releases)
- For some linux OS, rpm pack may not work, you can try the `.snap` release.
- For Mac user: `brew cask install electerm`
- With snap: `sudo snap install electerm`
- For Deepin Linux user, you can find it from App store.
- Install from npm

```bash
npm i -g electerm

# after install it will open at once for windows and linux,
# for mac, will open the drag to install panel

```

## Upgrade

- Auto upgrade: When new version released, you will get upgrade notification after you start electerm again, then you click the upgrade button to upgrade.
- Download: Just download the latest edition, reinstall.
- Npm: If you install from npm, just run `npm i -g electerm` again.

## Features

- Work as a terminal/file manager or ssh/sftp client(similar to xshell)
- Global hotkey to toggle window visibility (simliar to guake, default is `ctrl + 2`)
- Multi platform(linux, mac, win)
- 🇺🇸 🇨🇳 🇧🇷 🇷🇺 🇪🇸 🇫🇷 🇹🇷 Support multi-language([electerm-locales](https://github.com/electerm/electerm-locales), contribute/fix welcome)
- Double click to directly edit remote file(small ones).
- Edit local file with built-in editor(small ones).
- Auth with publickey + password.
- Zmodem(rz, sz).
- Transparent window(Mac, win).
- Terminal background image.
- Global/session proxy.
- Quick commands
- Sync bookmarks/themes/quick commands to github secret gist
- Serial Port support

## Support

Without users's feedbacks/suggestions/pull requests/language files, this project would not get this far, would love to hear from you, please tell me what you think, [submit an issue](https://github.com/electerm/electerm/issues), [send me an email](mailto:zxdong@gmail.com), [create/fix language files](https://github.com/electerm/electerm-locales) or create a pull requests, all welcome.

## Dev

```bash
# tested in ubuntu16.04/mac os 10.13 only
# need nodejs/npm, suggest using nvm to install nodejs/npm
# https://github.com/creationix/nvm
# with node 8.6+

git clone git@github.com:electerm/electerm.git
cd electerm
npm i

# start webpack dev server
npm start

# in a separate terminal session run app
npm run app

# lint
npm run lint

# code format fix
npm run fix
```

## Test

```bash
npm run pre-test
cp .sample.env .env
# then edit .env, fill your test host/username/password
npm run test
```

## Test build

```bash
# Tested only in ubuntu 16.04 x64
# Install yarn first(to do yarn autoclean)
# See https://yarnpkg.com/en/docs/install

# Build linux only with -l
npm i
npm run pre-test
npm run release -l
# visit dist/
```

## Use

- [Set autorun when login to os](https://github.com/electerm/electerm/wiki/autorun-electerm-when-login-to-os)

## Change log

Visit [Releases](https://github.com/electerm/electerm/releases).

## License

MIT
