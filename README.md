# BOLDER — editable website

This is the **ready-to-publish source** for BOLDER, built with Jekyll and designed to be edited using [Pages CMS](https://app.pagescms.org/). No need to edit HTML to add interviews.

## What is ready
- Original BOLDER logo and 3 portrait photos
- Fully written Muffie Grieve interview
- Homepage, People archive, About page and Book page
- Two unpublished interview drafts: Robert Burke and Alan Kitching (no interviews invented)
- Responsive design for desktop and mobile
- Pages CMS configuration (`.pages.yml`)

## Publishing it (one-time setup)
1. Make a free GitHub account at https://github.com if you don't already have one.
2. Make a **new public repository** called `bolder-site` (don't add a README).
3. Upload the **contents of this folder** to that repository. Important: include the hidden file `.pages.yml`. The easiest approach is to unzip this package and upload the files and folders using GitHub's **Add file → Upload files** control. GitHub's browser uploader may omit folders with hidden files or be awkward for many items; GitHub Desktop is an alternative.
4. In GitHub, choose **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root)**, then save. GitHub Pages builds Jekyll sites automatically. Your public site address will typically be `https://YOUR-USERNAME.github.io/bolder-site/`.
5. **Important for a project repository:** in `_config.yml`, set `baseurl: "/bolder-site"` before deployment. If you later use a custom domain, change `baseurl` back to `""` and set `url` to your domain.
6. Visit https://app.pagescms.org/ and sign in using GitHub. Authorise access to your `bolder-site` repository. Choose that repository.
7. Open **Interviews** to add an interview, upload a portrait, edit text and tick **Publish interview**; save. Changes are stored in GitHub and rebuild the public website.
8. Use the **About BOLDER** and **The book** sections to edit those pages in the same visual editor.

## Important notes
- This package is **not yet published**, and Pages CMS isn't connected until you've done the GitHub account setup and authorisation.
- This editable publishing version is different from the earlier plain-HTML offline preview. To preview the *source* locally, run Jekyll (requires Ruby). A quick way to see the visual design without installing anything is the earlier prototype zip.
- The hero headline and quote are currently hard-coded to Muffie. Keep Muffie featured unless we update the homepage copy for a different interview.
- Keep your original high-resolution photos backed up separately.
- The site uses no WordPress plugins and has no public login or writable database, reducing the maintenance and attack surface.
