# Kascade
The goal of Kascade is to keep a sites SASS folder & file structure consistent and it's code clean and well thought out. With that being said this model is not just for large sites with a huge code base. It should be used on any site you build whether it's a small one page website or large corporate site with hundreds of pages. The underlining idea of Kascade is to have consistency. Because the more consistent our SASS is, the easier it will be to maintain down the road.

##Benfits
- **Clean Hierarchy** - Kascade's file & folder hierarchy is structured in such a way that high-level & vendor code is located at the top of the code base and then cascades down to more specific low level code at the end of the code base. So no ~~!important~~!
- **Developer Friendly** - Another advantage of Kascade is a having a defined code structure. So when doing a code hand offs or when adding new developers to a project explaining the logic and structure is incredibly easy.

## Structure Overview
```html
Kascade
│   main.scss
│
└───00-Vendors
    │   __index.scss
    │
    01-base
    │   __index.scss
    │   _fonts.scss
    │   _grid.scss
    │   _mixins.scss
    │   _variables.scss
    |
    02-elements
    │   __index.scss
    │   _buttons.scss
    |   _forms.scss
    |   _general.scss
    |   _lists.scss
    |   _typography.scss
    |
    03-components
    |   __index.scss
    |   _footer.scss
    |   _header.scss
    |   _sidebar.scss
    |
    04-modules
    |   __index.scss
    |   _search.scss
    |   
    05-layouts
    |   __index.scss
    |   _full-width.scss
    |   _page.scss
    |   _post.scss
    |
    06-pages
    |   __index.scss
    |   _home.scss
    |
    07-helpers
    |   __index.scss
    |   _isMobile.scss
```
## Logic
Now to get down to business. As you may have noticed by now each folder has one file in common and that is **__index.scss**. This file contains all the @imports for that particular folder and in the end gets pulled in the **main.scss** file. Going back to the folders each folder has a numerical prefix on it. This is simply used to keep our folders in order and also help quickly visualize the folder structure. So now it's time to go folder by folder where the real magic happens.

### 00-vendors
This folder is for holding any 3rd party vendors files you might be using in your project. So for example Susy, normalize, ect.

_*You can view examples in the files inside the this folder._

```html
Kascade
│   main.scss
│
└───00-Vendors
    │   __index.scss
```

### 01-base
This folder is for all your projects base settings like fonts, grid settings, mixins, and variables.

_*You can view examples in the files inside the this folder._

```html
Kascade
│
└───01-base
    │   __index.scss
    │   _fonts.scss
    │   _grid.scss
    │   _mixins.scss
    │   _variables.scss
```

### 02-elements

```html
Kascade
│
└───02-elements
    │   __index.scss
    │   _buttons.scss
    |   _forms.scss
    |   _general.scss
    |   _lists.scss
    |   _typography.scss
```

### 03-components

```html
Kascade
│
└───03-components
    |   __index.scss
    |   _footer.scss
    |   _header.scss
    |   _sidebar.scss
```

### 04-modules

```html
Kascade
│
└───04-modules
    |   __index.scss
    |   _search.scss
```

### 05-layouts

```html
Kascade
│
└───05-layouts
    |   __index.scss
    |   _full-width.scss
    |   _page.scss
    |   _post.scss
```

### 06-pages

```html
Kascade
│
└───06-pages
    |   __index.scss
    |   _home.scss
```

### 07-helpers

```html
Kascade
│
└───07-helpers
    |   __index.scss
    |   _isMobile.scss
```
