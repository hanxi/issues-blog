# issues-blog

给使用 github issuse 作为个人博客设置单独界面。

### 使用步骤

1. 创建 repository，假设 repository 名字为 blog。或者 Fork 我这个 repository。
2. 创建 gh-pages 分支。
3. 把我这个 repository 下的文件拷贝到你的 gh-pages 分支下。
4. 修改 config.js 文件

  ```js
  config = {
      blog_name: "你的博客的名字",
      github_repo: "usename/repo"      // 你的 github 账号和 repository 的名字
  };
  ```

5. 然后就使用 https://username.github.io/blog （username 为你的 github 账号名，blog 为你创建的 repository 名字）访问你的博客了，博客内容是你这个 repository 下的所有 issues。
6. 可以修改 CNAME 使用域名访问你的博客
