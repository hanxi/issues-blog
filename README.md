# issues-blog

给使用 github issuse 作为个人博客设置单独界面。

### 使用步骤

1. 创建 repository，假设 repository 名字为 blog。或者 Fork 我这个 repository。
2. 创建 gh-pages 分支。
3. 把我这个 repository 下的文件拷贝到你的 gh-pages 分支下。
4. 修改 config.js 文件

    ```js
	config = {
	    blog_name: "涵曦 ● 博客",
	    github_username: "hanxi", // github 账号名
	    github_repo: "blog",      // github 建立的 repo 名
	    per_page: 10,             // 首页每次载入文章列表数量
        // 请求量大时需要在 github 后台单独设置一个读取公开库的 token
        // 将配置好的 access token 拆分成两个字符串相加
        access_token: "dbfe3dd66ee904988f2b"+"aaaf9bf49a03b6e3fd62"
	};
    ```
    
   * access_token 的申请参考这里 https://github.com/wuhaoworld/github-issues-blog
   * 一定要拆分字符串相加，否则 github 会自动使 access_token 实效

5. 然后就使用 https://username.github.io/blog （username 为你的 github 账号名，blog 为你创建的 repository 名字）访问你的博客了，博客内容是你这个 repository 下的所有 issues。
6. 可以修改 CNAME 使用域名访问你的博客

### 如何实现的？

http://blog.hanxi.info/?p=6
