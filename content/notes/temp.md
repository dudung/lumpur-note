+++
title = 'temp'
subtitle = 'List of students seminar for all programs'
link = 'https://osf.io/zqyb2'
version = '20240309_v1.1'
date = '2024-03-09T17:15:00+07:00'
draft = false
type = 'xtalk'
tags = ['osf']
authors = ['viridi']
url = 'osf/zqyb2'
+++
<!--more-->


$ git clone https://github.com/dudung/lumpur-note
Cloning into 'lumpur-note'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (4/4), done.


$ hugo new site lumpur-note -f
Congratulations! Your new Hugo site was created in M:\lumpur-note.

Just a few more steps...

1. Change the current directory to M:\lumpur-note.
2. Create or install a theme:
   - Create a new theme with the command "hugo new theme <THEMENAME>"
   - Or, install a theme from https://themes.gohugo.io/
3. Edit hugo.toml, setting the "theme" property to the theme name.
4. Create new content with the command "hugo new content <SECTIONNAME>\<FILENAME>.<FORMAT>".
5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.


$ hugo new theme lunote
Creating new theme in M:\lumpur-note\themes\lunote


$ rm -r themes/lunote/content/*


$ nano hugo.toml

baseURL = 'https://dudung.github.io/lumpur-note'
languageCode = 'en-us'
title = 'lumpur-note'
theme = 'lunote'

enableEmoji = true

[pagination]
pagerSize = 16

[taxonomies]
  author = "authors"
  tag = "tags"
  category = "categories"

[[menu.main]]
  name = 'Home'
  weight = 2
  identifier = 'home'
  url = '/'


