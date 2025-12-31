# Basic Site Settings
locale                  : "en-US"
site_theme              : "default"
title                   : "Kouyakou-Abalo SIMSOBA"
title_separator         : "-"
name                    : "Kouyakou-Abalo SIMSOBA"
description             : "Google DeepMind Scholar | AI for Science Researcher"
url                     : "https://simsoba-research.github.io"
baseurl                 : ""
repository              : "simsoba-research/simsoba-research.github.io"
repository_search       : false

# Site Author - Sidebar Profile
author:
  avatar                : "profile.png"
  name                  : "Kouyakou-Abalo SIMSOBA"
  bio: |
    Google DeepMind Scholar | M.Sc. Mathematics (PAUSTI, African Union Scholar) | MSc in AI for Science at Stellenbosch University 
  location              : "Cape Town, South Africa"
  employer: |
    AIMS, South Africa
  email                 : "kouyakou@aims.ac.za"

  # Academic and Professional Links
  googlescholar         : "https://scholar.google.com/citations?hl=en&user=RtYAMMoAAAAJ"
  orcid                 : "https://orcid.org/0009-0005-4050-5040"
  researchgate          : "https://www.researchgate.net/profile/Kouyakou-Abalo-Simsoba"
  github                : "Abalo39"
  linkedin              : "https://www.linkedin.com/in/abalo-simsoba-803a75244/"

# Publication Category Headings
publication_category:
  books:
    title: "Books"
  manuscripts:
    title: "Journal Articles"
  conferences:
    title: "Conference Papers"

# Site Settings
minimal_mistakes_skin    : "default" # FIXED: This line removes the gear icon
search                   : false     # FIXED: Prevents search icon placeholder
breadcrumbs              : false
words_per_minute         : 160
future                   : true
read_more                : "disabled"
talkmap_link             : false
comments:
  provider               : false

# File Management
include:
  - .htaccess
  - _pages
  - files
exclude:
  - "*.sublime-project"
  - "*.sublime-workspace"
  - .asset-cache
  - .bundle
  - .github
  - .jekyll-assets-cache
  - .sass-cache
  - assets/js/_main.js
  - CHANGELOG
  - LICENSE
  - node_modules
  - package.json*
  - README
  - vendor
keep_files:
  - .git
  - .svn

encoding: "utf-8"
markdown_ext: "markdown,mkdown,mkdn,mkd,md"

# Conversion
markdown: kramdown
highlighter: rouge
excerpt_separator: "\n\n"
incremental: false

# Collections
collections:
  teaching:
    output: true
    permalink: /:collection/:path/
  publications:
    output: true
    permalink: /:collection/:path/
  portfolio:
    output: true
    permalink: /:collection/:path/
  talks:
    output: true
    permalink: /:collection/:path/

# Defaults
defaults:
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: true
      read_time: true
      share: true
  - scope:
      path: ""
      type: pages
    values:
      layout: single
      author_profile: true
  - scope:
      path: ""
      type: teaching
    values:
      layout: single
      author_profile: true
      share: true
  - scope:
      path: ""
      type: publications
    values:
      layout: single
      author_profile: true
      share: true
  - scope:
      path: ""
      type: talks
    values:
      layout: talk
      author_profile: true
      share: true

# Styling
sass:
  sass_dir: _sass
  style: compressed

# Output
permalink: /:categories/:title/
timezone: Etc/UTC

# Plugins
plugins:
  - jekyll-feed
  - jekyll-gist
  - jekyll-paginate
  - jekyll-sitemap
  - jemoji

category_archive:
  type: liquid
  path: /categories/
tag_archive:
  type: liquid
  path: /tags/

compress_html:
  clippings: all
  ignore:
    envs: development
