# Java 练习项目

这个仓库可以存放多个独立的 Java 练习项目，并一起提交到 [GitHub 仓库](https://github.com/Ming-Light-Code/myjava-practice)。

## 当前目录

| 路径 | 内容 |
| --- | --- |
| `src/` | 最初的练习项目（仓库根目录） |
| `test2/` | 第二个独立项目 |

以后每新建一个项目，就在仓库根目录下新建一个文件夹，例如 `calculator/`、`student-manager/`。把该项目的 `src/`、`pom.xml` 或 `build.gradle` 等源码和构建文件放在自己的文件夹里。编译输出、IntelliJ IDEA 的本地配置会被忽略。

**新项目不要再执行 `git init`。** 所有项目共用根目录的 Git 仓库；如果 IntelliJ IDEA 提示为子项目创建 Git 仓库，请选择不创建。各项目可分别在 IntelliJ IDEA 中打开。

## 提交到 GitHub

在 PowerShell 中进入仓库根目录，然后运行：

```powershell
cd C:\Users\ming\Desktop\myjava-practice
git status
git add .
git commit -m "添加或更新 Java 项目"
git push origin main
```

提交前可以运行 `git status` 检查将上传的文件。若只想提交一个项目，可改用 `git add 项目文件夹名/`；根目录的练习代码使用 `git add src/`。

`test2/.git.previous/` 保留了 `test2` 原来独立 Git 仓库的历史，仅存在于本机，不会提交到 GitHub。当前仓库的 Git 历史位于根目录的 `.git/`。
