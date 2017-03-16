## 参考
- [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)
- [我的提交信息规范](http://yanhaijing.com/git/2016/02/17/my-commit-message/)

## 使用
```bash
$ git clone https://github.com/zhaotoday/commit-message.git
```

```bash
$ npm install
```

```bash
$ npm install -g commitizen conventional-changelog-cli
```

```bash
# 让项目支持 Angular 的 Commit message 格式
# npm install 安装所有 dev 依赖包后可不执行该命令
$ commitizen init cz-conventional-changelog --save --save-exact
```

```bash
# 替代 git commit 命令
$ git cz
# or
$ git commit
```

```bash
# 生成 Change log
$ npm run changelog
```

## 举个栗子
```
feat: 添加了分享功能

给每篇博文添加了分享功能

- 添加分享到微博功能
- 添加分享到微信功能
- 添加分享到朋友圈功能

Issue #1, #2
Close #1
```

## 相关包
#### commitizen
一个撰写合格 Commit message 的工具。

#### validate-commit-msg
用于检查 Node 项目的 Commit message 是否符合格式。

```bash
# 不会覆盖以前的 Change log，只会在 CHANGELOG.md 的头部加上自从上次发布以来的变动
$ conventional-changelog -p angular -i CHANGELOG.md -w
```

```bash
# 生成所有发布的 Change log
$ conventional-changelog -p angular -i CHANGELOG.md -w -r 0
```

#### husky
git 提交时的自动化处理。

#### conventional-changelog-cli
生成 Change log 的工具。
