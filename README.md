# ApiDoc
jazzy是一个命令行工具，用来生成 Swift 或 Objective-C 文档。


# 介绍

![使用Jazzy生成Html文档](%E6%88%AA%E5%B1%8F2022-04-24%20%E4%B8%8B%E5%8D%883.13.15.png)
# 使用Jazzy生成Html文档

## 1.  安装

```
sudo gem install -n /usr/local/bin jazzy
```

## 2.  cd到项目工程所在的文件夹，然后执行下面代码即可生成文档：

```
jazzy
```
默认位置为同一目录下生成的doc文件夹，如果想指定目录，使用:

```
jazzy -o 文档想存放的目录
```
也可以设置作者名：

```
jazzy -o 文档想存放的目录 --author 作者名
```

## 3. 其他事项
生成的文档是项目的主工程中的公开方法（里面有AppDelegate等文件的文档），Pods里的库的代码是不会生成的，因此如果是模块示例代码只想生成模块相关方法的文档，可以先将示例代码删除，将想要生成的代码直接加到主工程中（pod里的本地库先卸载），生成完成后再还原回去即可。


# 使用SourceDocs生成MarkDown文档
SourceDocs是一个命令行工具，可以从代码生成MarkDown文档文件。
## 1.  安装

```
brew install sourcedocs
```

## 2. 同样cd到项目文件夹下，执行：

```
sourcedocs generate
```
默认生成文档的位置在同一目录下的Documentation/Reference文件夹中，如果想要指定目录，使用：

```
sourcedocs generate --output-folder 文档想存放的目录
```

## 3.  其他事项

它们在生成文档时，都可以指定要生成文档的最低访问级别（默认为public），执行命令时添加如下代码即可：

```
--min-acl (private|fileprivate|internal|public|open)

```

如：

```
jazzy --min-acl internal

sourcedocs generate --min-acl internal
```
