A Github Pages template for academic websites. This was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

I think I've got things running smoothly and fixed some major bugs, but feel free to file issues or make pull requests if you want to improve the generic template / theme.

### Note: if you are using this repo and now get a notification about a security vulnerability, delete the Gemfile.lock file. 

# Instructions

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch. 

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20). Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.

# 使用记录
1. 主页侧边栏在 _config.yml 中更改
2. 主页内容在 /_pages/about.md 中更改
3. 顶部导航栏 在 /_data/navigation.yml 中更改，可以删掉不用的导航栏
4. publications
   1. 更改 /_publications 文件夹，向里面加入文件，文件名必须是 yyyy-mm-dd-paper-title-number-(1).md的形式，publications会自动添加记录
   2. 里面内容中的 permalink 设置为 /publication/文件名（不用.md）即可，跳转后进入的内容在该文件的md 中编写
   3. 有时候浏览器会有缓存，导致你修改了以后还是以前的设置，需要清空一下缓存

5. 插入图片，可以参考[issue](https://github.com/academicpages/academicpages.github.io/issues/140)，用这个插入图片需要第三方图床，我用的是[imgur](https://monaco12138.imgur.com/all)，上传到上面后选择image浏览模式导出图片的url后添加即可，直接传到github上会加载不出来。这一点还是挺麻烦的，要引入第三方来管理图片

   <img src="https://i.imgur.com/v6hqtH7.png" width="50%">

6. CV 在 /_pages/cv.md 中更改
7. Blogs 在/_posts/ 中添加md即可
   1. 文件名最好保持一致 yyyy-mm-dd-blog-post-(1).md，blogs会自动记录
   2. 里面的内容 permalink 设置为/posts/yyyy/mm/blog-post-(1)/ 的形式即可，跳转后的内容在该文件的md中编写
   3. tags添加可以用中文做记号