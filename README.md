# v-editor

[![Build Status](https://travis-ci.com/FEMessage/v-editor.svg?branch=master)](https://travis-ci.com/FEMessage/v-editor)
[![NPM Download](https://img.shields.io/npm/dm/@femessage/v-editor.svg)](https://www.npmjs.com/package/@femessage/v-editor)
[![NPM Version](https://img.shields.io/npm/v/@femessage/v-editor.svg)](https://www.npmjs.com/package/@femessage/v-editor)
[![NPM License](https://img.shields.io/npm/l/@femessage/v-editor.svg)](https://github.com/FEMessage/v-editor/blob/master/LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/FEMessage/v-editor/pulls)
[![Automated Release Notes by gren](https://img.shields.io/badge/%F0%9F%A4%96-release%20notes-00B2EE.svg)](https://github-tools.github.io/github-release-notes/)

Lightweight rich text editor based on [ckeditor5](https://github.com/ckeditor/ckeditor5) and [upload-to-ali](https://github.com/FEMessage/upload-to-ali).

![view.png](https://i.loli.net/2020/02/03/5J8Holf2vqrGSwu.png)

[中文文档](./README-zh.md)

## Table of Contents

- [Feature](#feature)
- [Demo](#demo)
- [Install](#install)
- [Quick Start](#quick-start)
- [Links](#Links)
- [License](#license)
- [Contributors](#contributors)

## Feature

- **File Upload** : Integrated upload components, just configure the basic information of OSS ([Configuration Reference](https://github.com/FEMessage/upload-to-ali/blob/dev/README.md#dotenv)), you can upload the picture or file to oss, support screenshot paste upload
- **Add Net Image**: Can quickly add a net picture using the markdown picture syntax(`![]()`), or you can paste it directly
- **Fullscreen Editing**: Allows the editor to cover the window

[⬆Back to Top](#table-of-contents)

## Demo

- [Doc and online demo](https://femessage.github.io/v-editor/)

[⬆Back to Top](#table-of-contents)

## Install

```sh
# Upload image function depends on upload-to-ali component
yarn add @femessage/upload-to-ali @femessage/v-editor
```

[⬆ Back to Top](#table-of-contents)

## Quick start

```html
<!-- step1 Ensure oss config -->
<!-- step2 In the .vue file that needs to use the -->
renderer
<template>
  <v-editor v-model="content" />
</template>

<script>
  import VEditor from '@femessage/v-editor'

  export default {
    components: {
      VEditor
    },
    data() {
      return {
        content: ''
      }
    }
  }
</script>
```

[⬆ Back to Top](#table-of-contents)

## Links

- [how to create a plugin](https://www.yuque.com/docs/share/d52c00bf-d379-45c6-955f-8eb218a4dabf?translate=en)

[⬆ Back to Top](#table-of-contents)

## License

[MIT](./LICENSE)

[⬆ Back to Top](#table-of-contents)

## Contributors

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table><tr><td align="center"><a href="https://github.com/kunzhijia"><img src="https://avatars2.githubusercontent.com/u/4848041?v=4" width="100px;" alt="kunzhijia"/><br /><sub><b>kunzhijia</b></sub></a><br /><a href="https://github.com/FEMessage/v-editor/commits?author=kunzhijia" title="Code">💻</a> <a href="https://github.com/FEMessage/v-editor/issues?q=author%3Akunzhijia" title="Bug reports">🐛</a> <a href="https://github.com/FEMessage/v-editor/commits?author=kunzhijia" title="Documentation">📖</a></td><td align="center"><a href="https://github.com/listars"><img src="https://avatars2.githubusercontent.com/u/20613509?v=4" width="100px;" alt="listars"/><br /><sub><b>listars</b></sub></a><br /><a href="https://github.com/FEMessage/v-editor/issues?q=author%3Alistars" title="Bug reports">🐛</a> <a href="https://github.com/FEMessage/v-editor/commits?author=listars" title="Documentation">📖</a></td><td align="center"><a href="https://donaldshen.github.io/portfolio"><img src="https://avatars3.githubusercontent.com/u/19591950?v=4" width="100px;" alt="Donald Shen"/><br /><sub><b>Donald Shen</b></sub></a><br /><a href="https://github.com/FEMessage/v-editor/issues?q=author%3Adonaldshen" title="Bug reports">🐛</a> <a href="https://github.com/FEMessage/v-editor/commits?author=donaldshen" title="Documentation">📖</a> <a href="#plugin-donaldshen" title="Plugin/utility libraries">🔌</a> <a href="#review-donaldshen" title="Reviewed Pull Requests">👀</a></td><td align="center"><a href="http://levy.work"><img src="https://avatars3.githubusercontent.com/u/9384365?v=4" width="100px;" alt="levy"/><br /><sub><b>levy</b></sub></a><br /><a href="#review-levy9527" title="Reviewed Pull Requests">👀</a> <a href="#infra-levy9527" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#ideas-levy9527" title="Ideas, Planning, & Feedback">🤔</a></td><td align="center"><a href="https://colmugx.github.io"><img src="https://avatars1.githubusercontent.com/u/21327913?v=4" width="100px;" alt="ColMugX"/><br /><sub><b>ColMugX</b></sub></a><br /><a href="https://github.com/FEMessage/v-editor/commits?author=colmugx" title="Code">💻</a> <a href="#blog-colmugx" title="Blogposts">📝</a> <a href="#design-colmugx" title="Design">🎨</a> <a href="#plugin-colmugx" title="Plugin/utility libraries">🔌</a></td></tr></table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
