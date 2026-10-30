Chunxi Zhao — GitHub Pages + Pages CMS 版本（2026-10）
================================================

这是基于你已经发布的网站制作的 Pages CMS 可编辑版本。
仍然使用你的原网站：https://chunxizhao.github.io/
网站设计基本保留；后续编辑个人介绍、项目、论文、工作经历、联系方式，无须修改 HTML。

一、第一次安装（只需一次）

1. 在 Windows 上解压本 ZIP 文件（不要把 ZIP 压缩包本身上传）。
2. 打开仓库 https://github.com/ChunxiZhao/ChunxiZhao.github.io
3. 点击 Add file -> Upload files。
4. 在 Windows 文件管理器中【进入解压后的文件夹】，全选其内部内容：
      index.html
      .pages.yml
      content 文件夹（里面含 4 个 json 文件）
      media 文件夹
      README_使用说明.txt
   然后把这些内容一起拖入 GitHub 的上传区域。
   重要：文件必须位于仓库根目录，不能多包一层文件夹；请先在网页上确认上传的路径。
   Github 官方支持拖入文件夹，并保留其中目录结构。
5. 看到文件列表后，确认 index.html 将更新，.pages.yml 位于根目录，content/site.json 等位于 content/ 下。
6. 点击 Commit changes -> Commit directly to the main branch。
7. 等 GitHub Pages 自动部署完成。网站视觉和原来类似。

二、连接 Pages CMS（只需一次）

1. 打开 https://app.pagescms.org
2. 点击 Sign in with GitHub，并使用 ChunxiZhao 账号登录。
3. 按提示安装/授权 Pages CMS 的 GitHub App。
4. 仓库选择：可以只授权 ChunxiZhao.github.io 这个仓库（推荐最小权限）。
5. 进入 ChunxiZhao / ChunxiZhao.github.io，选择 main 分支。
6. 你应该看到 4 个中文内容菜单：
      01 · 首页与联系方式
      02 · 项目 / Projects
      03 · 研究与工作经历
      04 · 论文 / Publications
   如果界面提示要创建 .pages.yml，说明配置文件可能没有被上传到仓库根目录。

三、以后怎么修改

- 修改名字/介绍/技能标签：01 · 首页与联系方式 -> 修改 -> Save。
- 添加/删除项目：02 · 项目 / Projects -> 在项目列表里增删；添加封面图片可直接用 Image 字段上传。
- 修改工作经历：03 · 研究与工作经历。
- 添加论文：04 · 论文 / Publications -> 添加论文条目、作者、期刊、年份和链接。
  注意：默认论文列表为空，所以网站上不会显示 Publications；添加第一篇后自动出现。
- 上传简历：在 01 · 首页与联系方式 的 PDF 简历字段里选择或上传 PDF。
  成功保存后，网站会自动出现 Download résumé 按钮。
- GitHub URL 可以留空；网站不会展示代码仓库链接。
- Save 会将更改写入 GitHub main；GitHub Pages 随后自动重新发布。
- 修改内容后请刷新网站；通常需要稍等片刻让新版本发布。

四、提醒

- Pages CMS 提供“表单式/内容式编辑”，不是像 Framer 那样在网页上拖动排版。
- 初次安装后修改文本、图片、项目和论文，不用碰 HTML。
- 如果你未来要更改网站布局和颜色，仍需改代码或换到其他网站编辑平台。
- 目前未替你上传任何实际简历、邮箱、个人照片或论文，避免公开未经确认的信息。
- 仓库为 Public，上传的图片与简历将对任何人公开；上传前检查个人信息及知识产权。
- 上传图片建议 JPG/PNG/WebP，图片一般尽量小于 2–3 MB，页面加载更快。
- 若你只有本地电脑临时预览 index.html，浏览器可能不允许读取本地 JSON；
  发布到 GitHub Pages 后，网页通过 HTTPS 读取 content 文件即可正常工作。

五、出问题如何检查

- CMS 里看不到 4 个编辑菜单：检查仓库根目录的 .pages.yml 是否存在、CMS 是否有仓库权限。
- 网站没有更新：确认保存到了 main，检查 GitHub 仓库的 Actions / Pages 部署情况，然后强制刷新 Ctrl+F5。
- 项目图片不显示：检查图片 URL 与 GitHub 仓库中 media/ 里的实际文件路径是否一致。
- 网站出现空白或无内容：先检查 content/site.json、content/projects.json 是否在对应路径。

官方资料：
Pages CMS 快速开始：https://pagescms.org/docs/quick-start/
Pages CMS 配置：https://pagescms.org/docs/configuration/
GitHub 上传文件：https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
