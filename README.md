# The Netherlands eScience Center Confeence - Symposium

Designed and developed by @ctwhome

[![Netlify Status](https://api.netlify.com/api/v1/badges/92956d3a-b930-4233-b8e9-82e37b0ac3f0/deploy-status)](https://app.netlify.com/sites/nlesc/deploys)

## Editing Content, Events and Blogs

* Most of the content on the website can be changed from the markdown files located inside the `content` folder.
* The menu links in the header and the mobile side panel can be edited inside the `menu-items.md`
* Adding events is as easy as copying the template (https://github.com/nl-rse/website/blob/main/content/202X-MM-DD-meetup.TEMPLATE.md), changing its content and place it inside the `/content/events/<temaplte.md>` location.
* When creating new blog posts, any markdown file located inside `/content/posts/<lowercase-post.md>` will be picked up automatically.
* IMPORTANT: all file names need to be "lowercase" in order to make [them work in Netlify](https://answers.netlify.com/t/support-guide-netlify-app-builds-locally-but-fails-on-deploy-case-sensitivity/10754). Example: `2019-07-09-nl-rse-2019.md`
* Any modifications in the files will trigger a GitHub action to build and deploy automatically to the live website. The changes will be live after a few minutes.

## Build Setup Locally

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# generate static project
$ yarn generate

# generate and local test
$ yarn generate && yarn start
```

For a detailed explanation of how things work, check out the [documentation](https://nuxtjs.org).
