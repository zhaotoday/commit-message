## 参考
- [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)

## 安装包

#### commitizen
一个撰写合格 Commit message 的工具。
```bash
npm install -g commitizen
```
让项目支持 Angular 的 Commit message 格式：
```bash
commitizen init cz-conventional-changelog --save --save-exact
```

#### validate-commit-msg
用于检查 Node 项目的 Commit message 是否符合格式。
```bash
npm install --save-dev validate-commit-msg
```
不会覆盖以前的 Change log，只会在CHANGELOG.md的头部加上自从上次发布以来的变动：
```bash
conventional-changelog -p angular -i CHANGELOG.md -w
```
生成所有发布的 Change log：
```bash
conventional-changelog -p angular -i CHANGELOG.md -w -r 0
```

#### husky
git 提交时的自动化处理。
```bash
npm install --save-dev husky
```

## conventional-changelog-cli
生成 Change log 的工具。
```bash
npm install -g conventional-changelog-cli
```


## 命令
```bash
git cz
```
