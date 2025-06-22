---
tags: docs
---
## Blog Creation Notes
I wanted a simple, free, and no-ads place to post things and reconnect with people without any noisy social networking crap.

I found and used this generous template: 
 - [@chadbaldwin's _Building a Free Blog with GitHub Pages in Minutes_](https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html)

You'll need some basic experience with HTML, Markdown, and GitHub to follow along and create your own.
---

## Steps
To get the same blog setup you see here: 
1. Follow these steps: [https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html](https://chadbaldwin.net/2021/03/14/how-to-build-a-sql-blog.html)
2. Remove some noise: 
	a. If you don't want the RSS feed stuff, comment out the following line under **plugins** in the `_config.yml`: `- jekyll-feed`
	b. Notice that a link to your index page shows up twice on every page: in the top left and on the top right. To remove the redundant index page nav item on the top right, convert all your headers in `index.html` to **strong**
3. Add the comments feature by using https://utteranc.es/
4. Add a **Resume** nav item by creating a couple new files: (Note: I repurposed @chadbaldwin's existing resume setup to "Writing Samples" instead) 
	a. In the `_includes` folder, create a `resume.html` file. 
		- Add the following line of code, followed by your html or markdown: `{%- assign resume = site.data.resume -%}`
	b. In your GitHub site's root folder (`_username_.github.io`), create a `resume.md` file.
		- Add the following block of code: (Note: I changed my title to Writing Samples)
		~~~
		---
		title: Resume 
		layout: default
		---
		{%- include resume.html -%}
		~~~
		
✨ What's Next: Someday I'll sit down and update the styles to make it my own!