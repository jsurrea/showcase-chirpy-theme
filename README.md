# Showcase Chirpy Theme

This is a fork of [Chirpy](https://chirpy.cotes.page/), a static website generator that empowers you to publish beautiful websites with markdown syntax. The original project is focused on building blog websites; I decided to give it a turn to support people who want to use the awesomeness and simplicity of the theme for showcasing their personal projects. 

This should be a good starting point for research groups, startups, project documentation or tech enthusiasts to share their work on the internet, or even to publish your personal portfolio and CV. After all, it's all markdown! Use it to give a professional look to your idea and iterate fast. With this theme, you can focus on the content, and rest assured that your website will look gorgeous ✨

## How to use this theme

This repository contains the complete code to generate the theme from scratch. If you're interested in adding documentation in GitHub Pages to your existing repository, check out [showcase-chirpy-easy-docs](https://github.com/jsurrea/showcase-chirpy-easy-docs).

Also, check out these amazing resources to better understand how Chirpy works:

- [Getting Started with Chirpy](https://jsurrea.github.io/showcase-chirpy-theme/getting-started/)
- [Write your first post](https://jsurrea.github.io/showcase-chirpy-theme/write-a-new-post/)
- [Showcase](https://jsurrea.github.io/showcase-chirpy-theme/text-and-typography/)
- [Customize the favicon](https://jsurrea.github.io/showcase-chirpy-theme/customize-the-favicon/)

To use this repository and create your website from scratch, start by [forking it](https://github.com/jsurrea/showcase-chirpy-theme/fork). For the repository name, you have two alternatives:
1. If you want this to be the personal webpage for you or your organization, fork the repo with the name `<username>.github.io`
2. If you want to create a page for a product or project, use whatever name suits your needs. The webpage will be located at `<username>.github.io/<project>`

After you have forked this repo, you should be able to just edit the files and see the live result. Please confirm that you have enabled GitHub Actions in your repository by going to the 'Actions' tab. A workflow (`.github/workflows/pages-deploy.yml`) will run each time you push a new commit to the main branch which will trigger a new deployment of your website. If you want to test your changes locally, check out [this section](#how-to-build-from-source), though be advised that it's not meant for newcomers and commiting your changes directly should be enough if you're confident with markdown!

There's a few elements that you can customize to make the website truly _yours_ (for example, the title). Head over to the following files and search for all the `TODO` tags, where you will find concise documentation and examples to use this theme to the max potential 😎
- `_config.yml`
- `_data/contact.yml`
- `_data/share.yml`
- `index.md`

Don't forget to add as many pages as you need! Just create new markdown files in the `_tabs` directory and you're good to go!

## How to build from source

> Most of the details of this section can be found in [this wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki/Development-&-Test-Environments) from the original theme repo.

Before starting you will have to either: (a) Install [Jekyll](https://jekyllrb.com/docs/installation/) in your machine or (b) Run a dev-container with the environment already set-up. The latter is recommended if you're familiarized with containerization, since it will ensure that you do not face OS-specific errors related to the installation process.

To start the Jekyll server, execute `./tools/run.sh`. On parallel, open a new terminal and execute `npm run watch:js` to rebuild any changes you make to the JavaScript files of the repository. Alternatively, if you installed Jekyll through Bundle, you can execute `bundle exec jekyll serve`.

If everything goes alright, just head over to `http://127.0.0.1:4000/showcase-chirpy-theme/` and you're done.

## How does this work?

If you have previous experience with Chirpy, this is an overview of the changes that I applied on this fork:
- Added support to show the Table of Contents (ToC) within the layout for `page` (huge shoutout to [rafisics](https://github.com/rafisics) who shared a guide on how to do this [here](https://github.com/cotes2020/jekyll-theme-chirpy/discussions/2241)).
- Changed the default layout of the tab elements to use the `page` layout.
- Changed the layout of the home page (`index.md`) to use the `page` layout as well.


## Contributions

Feel free to contribute with more awesomeness! This project is open to improvements of all kinds 😄 That said, there's a few things I believe would be very useful for the theme:
- Migrating features to other layouts (specially `page`). Think about search, comments, word count, etc.
- New layouts and components, pottentially useful for showcasing.
- Customization: Colors, icons, sizes, etc.
- Improved documentation and tutorials.

