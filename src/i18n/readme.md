# How to add translations

1. Copy the [en/](https://github.com/qmk/qmk_configurator/tree/master/src/i18n/en) folder
2. Rename it to the appropriate [language tag](https://www.w3.org/International/articles/language-tags/)
3. Edit each variable in the `.js` files to the appropriate word/phrase 
4. Edit the main [index.js](https://github.com/qmk/qmk_configurator/blob/master/src/i18n/index.js) to include
   ```js
   import <tag> from './<tag>';
   ```
   and
   ```js
     ...<tag>,
   ``` 
   in the correct spots, with `<tag>` replaced with your language tag/folder name.  
5. Open a [Pull Request](https://github.com/qmk/qmk_configurator/pulls)!
