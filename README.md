## 参考
- [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)

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

## 相关包
#### commitizen
一个撰写合格 Commit message 的工具。

#### validate-commit-msg
用于检查 Node 项目的 Commit message 是否符合格式。

```bash
# 不会覆盖以前的 Change log，只会在CHANGELOG.md的头部加上自从上次发布以来的变动
$ conventional-changelog -p angular -i CHANGELOG.md -w
```

```bash
# 生成所有发布的 Change log
$ conventional-changelog -p angular -i CHANGELOG.md -w -r 0
```

#### husky
git 提交时的自动化处理。

## conventional-changelog-cli
生成 Change log 的工具。

## 命令
```bash
git cz
```
