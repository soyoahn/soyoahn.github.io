---
tags: docs
---
## Blog Creation Notes
I wanted a simple, free, no-ads place to post things and reconnect with people without any noisy social networking crap.

I found and used this generous template: 
 - [@chadbaldwin's _Building a Free Blog with GitHub Pages in Minutes_](https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html)
 
**I take zero credit for anything you see here**--it's all [@chadbaldwin](https://github.com/chadbaldwin). I'm just sharing notes for some of the customizations I made. You'll need some basic experience with HTML, Markdown, and GitHub to follow along and create your own.

---

## Steps
To get the same blog setup you see here: 
1. Follow these steps: [https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html](https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html) <br>The rest of this is totally optional stuff I did in addition:
2. Remove some noise: 
	1. If you don't want the RSS feed stuff, comment out the following line under **plugins** in the **_config.yml**: `- jekyll-feed`
	2. Notice that a link to your index page shows up twice on every page: in the top left and on the top right. To remove the redundant index page nav item on the top right, convert all your <font color="#FF7A32">headers</font> in `index.html` to <font color="#FF7A32">bold</font> (Haven't had a chance to check if there's a smarter workaround.) 
	
3. Add the **Comments** feature by using [https://utteranc.es/](https://utteranc.es/). The form on that readme is how you generate the small snippet of code you include in your [`_includes/comments.html`](https://github.com/soyoahn/soyoahn.github.io/blob/4d45a93eb0e5d3e8518eb254974de5bd0bd8caab/_includes/comments.html).

4. Add a **Writing Samples** nav item by creating a couple new files: 
	1. In the `_includes` folder, create a `writingsamples.html` file. 
		- Add the following line of code, followed by your html or markdown: {% raw %}`{%- assign writingsamples = site.data.writingsamples -%}`{% endraw %}
	2. In your GitHub site's root folder (`_username_.github.io`), create a `writingsamples.md` file.
		- Add the block of code you see here: [https://github.com/soyoahn/soyoahn.github.io/blob/main/writingsamples.md?plain=1](https://github.com/soyoahn/soyoahn.github.io/blob/main/writingsamples.md?plain=1)
		Note: Writing Samples is just one example. You could make a "Resume" or "Portfolio" one if you prefer! Just change the naming in those two files, including the filenames. 
		
✨ What's Next: Someday I'll sit down and update the styles to make it my own!