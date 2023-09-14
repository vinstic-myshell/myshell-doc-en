# External Knowledge Base

The knowledge base serves as the robot's external brain, providing it with knowledge beyond ChatGPT and public datasets, enabling it to have stronger capabilities in specific fields.

Use cases: Access project documents/product documents to answer ad hoc questions from users/partners; access academic literature to become an expert in the field; access someone's blog or tweets to become a digital life; ...

Currently supported link types include:

* [Gitbook](https://www.gitbook.com/)
* [Docusaurus](https://docusaurus.io/)
* Regular web pages

Support for more input formats (offline documents, text, Notion) is under development.

## How to start using the knowledge base function?

In the robot's editing page, click 'Knowledge Base' to start connecting the robot to an external knowledge base.

![](<../../.gitbook/assets/image (23).png>)

## How to make the knowledge base better serve the robot?

1. Use text-based web pages as much as possible. For large text-based web pages, Myshell's knowledge base can parse and respond well. Conversely, if it is a non-structured web page (such as a pure table, with many images and complex formats), Myshell's knowledge base may be a bit inadequate.
2. The multiple knowledge bases imported are of the same type. For robots that have imported multiple knowledge bases, if different knowledge bases are of the same type or have similar content, better results can be achieved. For example, if we want to create a robot for a certain anime character and use the knowledge base to supplement information about the anime and its worldview, if we need to import multiple knowledge bases, it is best to import those related to the anime.

## Tips

#### Tips for using Gitbook

Gitbook is an important way to feed the bot's knowledge base.

Website: [https://app.gitbook.com/](https://app.gitbook.com/)&#x20;

The content organization can refer to MyShell's official documentation [https://docs.myshell.ai/](https://docs.myshell.ai/)&#x20;

Editing page:

[Note] When writing/pasting/importing text content into the gitbook page, multimedia content such as attached files, online links, images, and audio cannot be read.&#x20;

[Note] You need to create a page in the Team Space. If you create a page in the Private Space, there will be permission issues when sharing.

[Content Writing] Organize content in a modular way, similar to writing Notion documents/Feishu documents/Google documents. When organizing content, you generally only use the following blocks in "commands".

[Page Hierarchy] If the content hierarchy is complex, you can create different pages in the left page editing bar.

[Page Sharing] Click "Share" in the upper right corner of the editing page to open the "Publish to the web" button, and then click "Copy published link" in the lower left corner to paste the link into the place where the app.myshell.ai robot requires the gitbook link.

[Content Update] After the page is publicly released, "Share" in the upper right corner of the page will be changed to "Edit". If you need to edit the content, you can click "Edit" to enter the editing page. After editing, click "Merge", and the updated content will be automatically synchronized.

#### Fill your bot with fresh knowledge base in 5 minutes | Easily grab network materials

1. **Grab the webpage and get the material**: HTTrack Website Copier. Just enter the webpage you want to grab, and this tool will download all the content of this webpage and its sub-webpages. Tool download link: [https://www.httrack.com/page/2/](https://www.httrack.com/page/2/)&#x20;
2. **Import to Gitbook and feed in batches**. The content captured by the small tool is in html format. You need to copy all the required html to a folder, compress it into a .zip file, and then use Gitbook's batch import function! (Already edited)

**Q: What should I do if the content captured by HTTrack is incomplete?** For example, a main site has several sub-links, and each sub-link is the required content. When there is too much content, HTTTrack cannot extract all the sub-link content.&#x20;

**A: At this time, you need to first obtain all the sub-links you need to obtain**, and then use HHTrack to crawl them one by one.&#x20;

**Method 1:** Use the Sitemap function to get all the links on the website, and filter out the pages you need. How to create a Sitemap, use plugins or online websites: [https://www.xml-sitemaps.com/](https://www.xml-sitemaps.com/) The filtering process can be done manually or automatically, and if there is too much content, you can ask the bot to write a small script to solve it (Figure 1).&#x20;

**Method 2:** Use the browser plugin Easy Web Data Scraper to get all the links. You need to set the crawling method and loading method simply, and it will crawl automatically. Link: [https://chrome.google.com/webstore/detail/easy-web-data-scraper/mndkmbnkepbhdlkhlofdfcmgflbjggnl](https://chrome.google.com/webstore/detail/easy-web-data-scraper/mndkmbnkepbhdlkhlofdfcmgflbjggnl)&#x20;

**Method 3:** For crawling with less content, use the plugin Link Gopher. If the links you need to crawl can be loaded on one page, this plugin can extract them most easily. Link: [https://sites.google.com/site/linkgopher/](https://sites.google.com/site/linkgopher/)