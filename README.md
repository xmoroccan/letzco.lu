# Letzco.lu documentation

As we know we can re-generate the website anytime we have some modifications, so in this documentation we gonna walk throuth the process, first let's begin with the structure:

## Folders structure

in this section we will not gonna mention all folder, insted we will focus on some of them (important)


FOLDER NAME  | DESCRIPTION
------------ | -------------
`_include`   | This folder contains website parts, if you need to correct some syntax mistake you will find those section here, probably you won't edit it!     
`_services`   | This folder is the important one because it contains each service content and other information variables, we gonna explain it later.
`_refrences`  | This folder also is important, here we gonna create our references, you can simply treat it as services folder, but with deferent variables.  

## How to

In this section, we gonna describe how you can create or edit website pages, let's start!

### Create new service
Create a new page is easy as creating a new file, if you check `_services` you will find three **subfolders** represent each branch:
- `communication-web`
- `securité`
- `sauvegarde`

 so to create a new service simply create a new file within `_services` **subfolders**, with the following:

```markdown
---
title        : Service title ex: "Création de sites web"
category     : Service category ex: "communication-web"
order        : Service Sort ex: 1
description  : Service description
thumbnail    : Service thumbnail
header_bg    : Service large image
card_color   : The color chosen for this service
---

And Here place service content!
```

Variable | required | role  
---------|----------|------  
title  | **true** | Service title, remember to place it inside the quote marks `""`.
category  | **true**   | Service category, for now the possible values is: `"communication-web"`, `"securité"` or `"sauvegarde"`.
order  | **true**  |  This is a numeric variable (1, 2, 3, 4...), to control services sorting within a branch
description  | **true**  | Short description used in a several parts on the website, remember short mean: `150 chars < total characters < 255 chars`, and remember to place it inside the quote marks `""`.
thumbnail  | **true**  | Thumbnail image to represent the service on index page, you can use any link inside the quote marks ex: `"https://www.somewebsite.com/some_image.jpg"` or upload it to `img/services/` and use `"/img/services/image_name.png"`.


title        : Service title ex: "Création de sites web"
category     : Service category ex: "communication-web"
order        : Service Sort ex: 1
description  : Service description
thumbnail    : Service thumbnail
header_bg    : Service large image
card_color   : The color chosen for this service
---
