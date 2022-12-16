# WWU Association for Gender Inclusion in Computing

This website is made with Hugo and based on the theme roxo-hugo.

The project structure is as follows:

- content
  - collection of files (.md) representing all content sections
    - if you want to add text content to the site, add it here
  - organized like the content on the rendered site
- data
  - config files (.yml) for different types of site content
- layouts
  - templates (.html) that specify how views of the content will be rendered into a static website
    - template for content structure on page
- static
  - all static content that gets copied directly into the hugo site upon generation
  - in this case, images
- assets
  - stores files to be processed by Hugo Pipes
  - in this case, stylesheets (.scss)
- config.toml
  - important file that configures settings for the whole site
- public
  - static site contents
  - generated with the bash command `hugo`
  - *updates are not self-propagating; this directory needs to be re-generated anytime updates are made to other hugo files*
- themes
  - themes added as submodules, in this case roxo-hugo
- resources
  - automatically generates and caches files
  - in this case, styles from assets/
- archetypes
  - templates (.md) for new content files
    - template for content text & metadata on page
  - (not really used for this project)

To run a dev server with this site: `hugo server`

Please don't push changes directly to the main branch. Make your changes to the dev branch, verify that nothing is broken, and then merge them to the main branch.
