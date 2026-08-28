DING GROUP WEBSITE — EDITING AND HOSTING GUIDE
===============================================

FILES
-----
index.html
  The complete website, including its styling.

assets/dawei-ding.jpg
  The portrait displayed on the website.

CNAME
  Tells GitHub Pages to use www.quantumtelepathic.com.


HOW TO EDIT
-----------
1. Make a backup copy of this folder.
2. Open index.html in a text editor.
3. Search for the text you want to change.
4. Edit only the text between HTML tags unless you are comfortable editing HTML.
5. Save the file.
6. Double-click index.html to preview it in a browser.

For example:

  <h1>David (Dawei) Ding</h1>

can be changed to:

  <h1>Your new heading</h1>


HOST WITH GITHUB PAGES
----------------------
1. Create a free GitHub account at https://github.com if needed.
2. Create a new PUBLIC repository, for example "ding-group-website".
3. Upload index.html, CNAME, and the assets folder to the repository.
4. Open the repository's Settings.
5. Select Pages.
6. Under "Build and deployment", choose "Deploy from a branch".
7. Select the main branch and the root folder, then save.
8. In the Pages custom-domain field, enter:

   www.quantumtelepathic.com

9. Wait for GitHub to show the DNS instructions.
10. At NameSilo, replace the existing "www" CNAME target with the GitHub target
    shown in the Pages settings. It will normally look like:

    YOUR-GITHUB-USERNAME.github.io

11. Remove the two OpenAI verification TXT records after the move is complete:

    _openai-site-verification.www
    _cf-custom-hostname.www

12. Return to GitHub Pages and enable "Enforce HTTPS" when it becomes available.


IMPORTANT
---------
Keep the OpenAI-hosted version and its DNS records in place until GitHub Pages
has finished publishing. Change the NameSilo DNS only after the GitHub copy is
ready. This avoids unnecessary downtime.

Owning a domain and hosting a website are separate. NameSilo continues to
manage the domain registration and DNS, while GitHub Pages serves these files.
