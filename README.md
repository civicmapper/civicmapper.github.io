# Civic Mapper LLC website (v.4.0)

This site was built using the *Agency Jekyll theme*,  based on [Agency bootstrap theme ](http://startbootstrap.com/templates/agency/)

===

# Dynamic Content

## Blog/News/Labs

Blog/News/Labs posts written as `markdown` files in `/_posts`.

The naming convention of these files is important, and must follow the format: `YEAR-MONTH-DAY-title.md`. The `permalinks` can be customized for each post, but the date and markup language are determined solely by the file name.

Corresponding header images and thumbnails should be saved to `assets/img/posts`.

Thumbnail for posts are shown on the home page. These should be 400x300 px and should be saved with high compression for fast loading.

## Projects / Portfolio

Projects are contained in `_data/projects.yml`. Supporting images should be saved in `assets/img`.

Thumbnail for projects are shown on the home page. These should be 400x300 px and should be saved with high compression for fast loading.

## Team

Team members and info are added via  `_data/contact.yml`. Team member images should be saved to `assets/img/team/`.

=========

For more details on Jekyll, read [documentation](http://jekyllrb.com/), specifically docs on [directory structure](https://jekyllrb.com/docs/structure/), which explain where files need to be and how to use liquid templates in order to generate the site.
