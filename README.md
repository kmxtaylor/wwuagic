# WWU Association for Gender Inclusion in Computing (Source Code)

This project is the source code that generates the [static AGIC website](https://github.com/kmxtaylor/wwuagic). It is made with Hugo and based on the theme roxo-hugo.

The project structure is as follows:

- content
  - collection of files (.md) representing all content sections
    - if you want to add text content to the site, add it here
  - organized like the content on the rendered site
- data
  - config files (.yml) for different types of site content
    - including variables for text and other values like image source paths
- layouts
  - templates (.html) that specify how views of the content will be rendered into a static website
    - template for content structure on page
- static
  - all static content that gets copied directly into the hugo site upon generation
  - in this case, images
- config.toml
  - important file that configures settings for the whole site
- themes
  - themes added as submodules, in this case roxo-hugo
  - styles sourced from here (in this case, a fork)
    - to edit styles, you should edit the nicely-organized SCSS in the [forked repo](https://github.com/kmxtaylor/roxo-hugo). Otherwise you may end up with style conflicts.
- resources
  - automatically generates and caches files
  - in this case, styles from assets/
- archetypes
  - templates (.md) for new content files
    - template for content text & metadata on page
  - (not really used for this project)
- public
  - static site contents
  - generated with the bash command `hugo`
  - not stored in this GitHub repo, but rather a [separate one](https://github.com/kmxtaylor/wwuagic)
  - *updates are not self-propagating; this directory needs to be re-generated anytime updates are made to other hugo files*

To run a dev server with this site: `hugo server`

Please don't push changes directly to the main branch. Make your changes to the dev branch, verify that nothing is broken, and then merge them to the main branch.

For editable copies of static files, please see Website folder of Google Drive.
