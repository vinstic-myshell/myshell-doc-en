# Knowledge Base

## Introduction to Knowledge Base

The knowledge base is like an external brain for robots, providing them with knowledge beyond the large language model, giving robots more accurate information and stronger capabilities in specific fields.

**The knowledge base has a wide range of applications**:

* Access to project/product documentation for precise Q&A.
* Access to academic literature to become a domain expert.
* Access to blogs/tweets to build a digital life.
* Access to game/animation wikis for high-precision role-playing.
* ...and more application scenarios as you can imagine!

## How to Use the Knowledge Base?

In the robot's editing page, go to the "Knowledge Base" panel in "Advanced Settings", turn on the knowledge base switch, and import the link to connect the robot to the knowledge base.

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Currently supported link contents include:

* [Gitbook](https://www.gitbook.com/)
* [Docusaurus](https://docusaurus.io/)
* Ordinary web pages with text content as the main content

More input support is under development, so stay tuned.

If you have a large amount of text content that requires multi-level parsing, please use [Gitbook](https://www.gitbook.com/) or [Docusaurus](https://docusaurus.io/). If you only need single-level parsing, import any text-rich web page.

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

When you import, the status will first show "Importing", indicating that the web page is being parsed.

After the import is successful, the status changes to green "Active", and you can use the knowledge base function normally!

If the import fails and shows "Invalid", you need to check the validity of the input link. If you enter a Gitbook link, please check if the link you imported is publicly available first.

### Precautions for Using the Knowledge Base

1. Only the pure text part will be used as the knowledge base content. Multimedia content such as files, online links, images, and audio attached to the page cannot be read at present.
2. Import natural language text paragraphs as much as possible and avoid complex formatted content such as tables.
3. When importing multiple knowledge bases, try to import knowledge bases with close relationships, which can achieve better results.

### Tips for Using Gitbook

Gitbook is an important way to feed the bot's knowledge base. You can use it to edit structured knowledge bases and input a large amount of information. It is recommended that you use a format similar to the official documentation of MyShell for content organization.

Usage:

1. Create a "Space" in Gitbook and edit documents inside the "Space".
2. You can import a large amount of content through Gitbook's "Import content", or manually edit the knowledge base.
3. If the content hierarchy is complex, you can create a "Subpage" in the left sidebar.
4. When the knowledge base content is completed, click "Share" in the upper right corner, open "Publish to the web", and copy the link you obtained.
5. Copy and paste the link to the MyShell knowledge base interface and click import.
6. When the knowledge base is successfully parsed, the green "Active" will appear below.

Now, you have successfully imported a large amount of information through Gitbook!

If you need to modify the knowledge base content, you can click "Edit" to enter the editing page. After editing is completed, click "Merge", and the updated content will be automatically synchronized to your robot.