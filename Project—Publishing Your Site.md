# Project 1
## Publishing Your Site
This activity builds on [last week's Local Website activity](Activity—Local%20Website.md) to publish your work to the world wide web!

Goal: Publish an HTML page to the web server of your choice.

Tip: If you use `<img>`, you must also upload the images to the server so that other people can see them! It's best practice to upload images to your own server so that you're not using someone else's bandwidth.

### Level 1—Neocities
**Best for beginners! Includes HTML walkthrough to publish index.html, good review of what we covered last week!**

*Neocities is a revitalization of popular 00's webhost "Geocities". By creating a free account, you will be issued a subdomain (`username.neocities.org`) as a web URL you can share with the public. Your content is hosted on Neocities' servers, which support HTML, CSS, and Javascript.*
1. Create a free account on [Neocities](https://neocities.org/)
2. Use the HTML Editor to publish `index.htm`
	1. Follow the HTML tutorial!
3. Share a screenshot with the class!
4. Share your Neocities URL

Suggestion: Maintain your files in your local system with Atom, in case the online code editor has an error. That way, you won't lose your work. Just copy + paste to Neocities every time you want to upload a change!

### Level 2—Netlify
**Good if you want to learn how to use Github for version control**

*Netlify supports HTML, CSS, Javascript, and Ruby. Sync files to your Github repository from your local computer, and they'll automatically push to your Netlify website. Your URL will be `random.netlify.app`*
1. Create a Github account if you haven't already
2. Create a new, empty repository on Github
3. Create a free [Netlify](https://www.netlify.com/pricing/) account
4. On Netlify, create a new [Netlify site from Git](https://docs.netlify.com/configure-builds/repo-permissions-linking/) and select Github as your provider.
6. Allow Netlify to access the Github repository you created in Step 2
7. On Github, verify that the Netlify app is installed properly (see image below)
8. Upload `index.htm` to your Github repository using any of these methods:
	1. On github.com, click `Add File > Create New File` and type your HTML manually in the browser
	2. On github.com, click `Add File > Upload Files` and upload an HTML document from your computer
	3. Install [Github Desktop](https://desktop.github.com/) and use it to auto-sync HTML files from a folder on your computer as you work on them through Atom (or other code editor)
9. Visit your Netlify dashboard and locate your Netlify URL
10. Visit your Netlify URL and you should see `index.htm` !
11. Share a screenshot with the class!
12. Share your Netlify URL

#### Netlify Bonus
*Custom Domain Name*
1. [Add a domain](https://docs.netlify.com/domains-https/netlify-dns/#add-a-domain) you own to Netlify
2. Follow Netify's instructions to update DNS records with your domain registrar

### Level 3—Github
**Harder to set up than Netlify, but has more free space & bandwidth**

*Github Pages supports HTML, CSS, Javascript, and Jekyll. Your URL will be `username.github.io`*
1. Create a Github account if you haven't already (**Important: Your Github username will become your URL, so change your username now if you're not happy with it**)
2. Create a new **public** repository on Github named **username.github.io**
	1. Important! Replace **username** with your username or it won't work!
3. Click `Settings > Github Pages` to make sure Github Pages is working
	1. If it's not, read my [instructions for Github Pages](https://github.com/coding-for-designers/ICD-Course-Reader/blob/main/Tutorials/Github%20Deployment.md) for the most common errors and how to fix them
4. Upload `index.htm` to your Github repository using any of these methods:
	1. On github.com, click `Add File > Create New File` and type your HTML manually in the browser
	2. On github.com, click `Add File > Upload Files` and upload an HTML document from your computer
	3. Install [Github Desktop](https://desktop.github.com/) and use it to auto-sync HTML files from a folder on your computer as you work on them through Atom (or other code editor)
5. Your site should be available on **username.github.io** !
11. Share a screenshot with the class!
12. Share your Github Pages URL

#### Github Pages Bonus
*Custom Domain Name*
[Instructions here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)

### Level 4—Self Hosting
**Good if you want to learn how to work with PHP apps such as Wordpress**

By buying your own webhosting plan, your bandwidth will not be throttled. This is recommended for your personal website if you want to have good uptime, want to upload lots of photos, or you anticipate growing your site to several thousand pageviews per month. Or if you just want to run on a green web host, since none of the free options are 100% renewable!

This is the only option that costs money for hosting. Custom domain names will always cost money as a separate fee and can be through a different company than your webhost (aka server) company. Most Shared hosting plans support HTML, CSS, Javascript, PHP, and MySQL.

I like using [Krystal UK](https://affiliate.k.io/go/QTbUFQzLFL)[^1] because it runs on 100% renewable energy (hydro, wind, solar). I use [Cyberduck](https://cyberduck.io/) (free FTP software) to upload files to the server. For domain registration, I usually use Dreamhost because they have super low prices and run on partially renewable energy.

[^1]: Affiliate link. Use code `megumi10` for £10 off

### Pick your favorite!
If you made it all the way to the end, you've gotten a great introduction to the different webserver options that exist today. You may have already gotten a feel for which interface or workflow you prefer, but if not, no worries! I often choose a server based on the tech stack and what sort of software I'd like to run on the server. Throughout this class, we will only be using HTML and CSS, so any of these options will work great for your personal site!

**Tips:**
- Think about `index` as an archival endeavor.
- What information are you archiving on your site? Is it an index of your class projects? Your web inspiration? A list of things you want to learn or create?
- Is it a list of your friends' websites? Books you've read this year or plan to read?
- Is it a log of what you did each week in class? (This is a great way to retain information!)
- Leave space for things you haven't made yet. For example, "What I learned in Week 2—_coming soon_"
