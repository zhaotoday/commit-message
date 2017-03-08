## 参考
- [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)

## commitizen

安装：
```bash
npm install -g commitizen
```

让项目支持 Angular 的 Commit message 格式：
```bash
commitizen init cz-conventional-changelog --save --save-exact
```

提交：
```bash
git cz
```

## validate-commit-msg
