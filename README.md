# ApiDoc

# 介绍
使用Jazzy生成Html文档
![使用Jazzy生成Html文档](%E6%88%AA%E5%B1%8F2022-04-24%20%E4%B8%8B%E5%8D%883.13.15.png)
# 安装教程

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


#### 使用说明

1.  xxxx
2.  xxxx
3.  xxxx

#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request


#### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
