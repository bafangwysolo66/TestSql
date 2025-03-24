# [工具名称] - [TestSql]

# 一、作者声明

我是一名专注于网络安全技术的探索者。这是我刚学Python安全工具开发不久所敲的一个用来测试sql注入的扫描器（拿来测试玩的😄），请各位师傅大佬们勿喷！本工具仅用于合法授权的安全测试与研究，任何未经授权的使用行为均与本人无关。

# 二、工具使用

由于在写的时候未添加 ArgumentParser ，所以感兴趣的师傅们可以直接在编辑器里面打开使用，毕竟是用来测试的，所以就偷个懒了哈哈哈。

SQL注入手动：
1.sql注入的原理是，判断有无后面我们自己输入的被带入sql语句执行
2.咱们常见的就是看到url之后先是无脑 '" and 1=1 测试一下是不是（反正我是😄），开玩笑的，师傅们的水平这么高，怎么可能和我一样呢（我是菜菜😄）
3.看网页的反应，有没有报错，或者通过时间猜测是否带入我们输入的参数

这里以著名的sqli-labs靶场进行测试：

<img width="1126" alt="sql" src="https://github.com/user-attachments/assets/123a2623-5861-4d4f-8b04-f91c4e93829d" />


<img width="637" alt="sql_code" src="https://github.com/user-attachments/assets/fdfcb811-5490-48e4-87e5-30512d7aeef6" />


简单写了一些常见的数据库报错提示，然后就是在url后面添加 ’ 和 “ 进行测试，是不是看起来很简单，相信各位师傅大佬们也能写出来。

最后就是测试啦：

<img width="879" alt="result" src="https://github.com/user-attachments/assets/9bdc55d4-a3b9-4750-b131-1a07af110525" />
