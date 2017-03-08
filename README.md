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

#### husky
用于处理 git 提交时的自动化处理。
```bash
npm install husky --save-dev
```

## 命令
```bash
git cz
```
