# [Aya Blogs](https://aitoricore.github.io/Aya-Blogs/)

这是一个基于 Hugo 的个人博客项目，当前使用 Terminal 主题，并对首页、文章列表、分页和部分样式做了简单自定义。

以下和以上内容均使用生成式人工智能生成。建议你仅供参考。

## 项目特点

- 基于 Hugo 静态站点生成器构建
- 支持中文内容组织，包含文章、日志、友链和标签页
- 自定义了首页布局、文章摘要、分页样式和部分模板
- 适合用于个人博客、技术记录和日常随笔

## 环境要求

建议安装 Hugo Extended 版本。

- Hugo 官方文档：https://gohugo.io/
- 安装完成后，确认版本：

```bash
hugo version
```

## 安装与运行

1. 克隆项目

```bash
git clone <你的仓库地址>
cd ayablog
```

2. 初始化子模块（如有需要）

```bash
git submodule update --init --recursive
```

3. 启动本地预览

```bash
hugo server -D
```

随后在浏览器中访问：

```text
http://localhost:1313
```

4. 生成静态站点

```bash
hugo
```

生成结果会输出到 public/ 目录。

## 项目结构

```text
archetypes/        # 内容模板
assets/           # CSS / JS 资源
content/          # 博客内容
  friends/         # 友链页
  log/             # 日志页
  posts/           # 文章内容
  tags/            # 标签页
layouts/          # 自定义模板与局部模板
  _default/       # 页面模板
  partials/       # 可复用片段
  shortcodes/     # 短代码
static/           # 静态资源，如图片、文件等
themes/           # 主题目录
public/           # 构建后的静态站点输出
hugo.toml         # Hugo 配置文件
```

## 内容编辑

- 新文章可以放在 content/posts/ 下
- 新页面可以在 content/ 对应目录中创建
- 站点标题、副标题、主题配置可在 hugo.toml 中修改
- 首页和文章列表样式可在 layouts/ 和 assets/ 中调整


