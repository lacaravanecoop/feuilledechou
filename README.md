# La Feuille de chou.
Email template for lacaravanecoop newsletter, "La feuille de chou" ; integrated upon [mjml](https://mjml.io) templating engine.

##Requirements :
- Git and Git Flow
- Node (14.2.0) and npm(6.14.4) (via [Node Version Manager](https://github.com/nvm-sh/nvm))

##Includes :
- MJML to HTML generation
- images optimisation

##Installation :

###Get the repo
``` bash
$ git@github.com:lacaravanecoop/feuilledechou.git ./feuilledechoux
```

###Install dependencies
``` bash
$ npm install
```

##Tasks

All the tasks works the same. Files from "src" folder are processed and generated in the dest directory.

###Build
Standalone build
``` bash
$ npm run build
```

###Watch
Build as any "src" files are modificated
``` bash
$ npm run watch
```

##Workspace
``` bash
-
|--cli
|--|--imagemin.js     # Imagemin task for image optimisation
|
|--dest               # Destination folder after build run (not to be edited)
|--|--assets          # Assets destination folder (images)
|--|--index.html      # Generated HTML mail file
|
|--src                # Source folder
|--|--assets 
|--|--|--images       # Image sources
|--|  
|--|--parts           # External MJML files
|--|--|--content      # External MJML files dedicated to contents
|--|--|--structure    # External MJML files dedicated to email structure
|--|
|--|--index.mjml      # Main MJML file
|
|--.gitignore         # All git ignored file on the project
|--.nvmrc             # Node Version environnement file on the project
|--package.json       # Project infos and dependencies
|--package-lock.json  # Project dependencies structure
|--README.medium      # The file You read actually
-
```

#Next steps
tests, tests and retests

Kisses and love, anvy questions or suggestions are welcome.