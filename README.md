# git
git experiment


## 用户信息

第一个要配置的是你个人的用户名称和电子邮件地址。这两条配置很重要，每次 Git 提交时都会引用这两条信息，说明是谁提交了更新，所以会随更新内容一起被永久纳入历史记录：

```sh
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

## 映射作者

如果文件.mailmap存在于存储库的顶层，或者位于mailmap.file或mailmap.blob配置选项所指向的位置，则它用于将作者和提交者名称以及电子邮件地址映射到规范的真实姓名和电子邮件地址。

在简单形式中，文件中的每一行都包含作者的规范实名，空格以及提交中使用的电子邮件地址（由<和>括起来）以映射到名称。例如：

```
Proper Name <commit@email.xx>
```