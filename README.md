# api documentation for  [diacritics (v1.3.0)](https://github.com/andrewrk/node-diacritics#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-diacritics.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-diacritics) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-diacritics.svg)](https://travis-ci.org/npmdoc/node-npmdoc-diacritics)
#### remove diacritics from strings

[![NPM](https://nodei.co/npm/diacritics.png?downloads=true)](https://www.npmjs.com/package/diacritics)

[![apidoc](https://npmdoc.github.io/node-npmdoc-diacritics/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-diacritics_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-diacritics/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-diacritics/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-diacritics/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrew Kelley"
    },
    "bugs": {
        "url": "https://github.com/andrewrk/node-diacritics/issues"
    },
    "dependencies": {},
    "description": "remove diacritics from strings",
    "devDependencies": {},
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "3efa87323ebb863e6696cebb0082d48ff3d6f7a1",
        "tarball": "https://registry.npmjs.org/diacritics/-/diacritics-1.3.0.tgz"
    },
    "gitHead": "a58b04da01ce92f1635918fef563e3286ea5a32e",
    "homepage": "https://github.com/andrewrk/node-diacritics#readme",
    "keywords": [
        "diacritics",
        "remove",
        "removal",
        "search",
        "string"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "superjoe",
            "email": "superjoe30@gmail.com"
        }
    ],
    "name": "diacritics",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/andrewrk/node-diacritics.git"
    },
    "scripts": {
        "test": "node test/test.js"
    },
    "version": "1.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module diacritics](#apidoc.module.diacritics)
1.  [function <span class="apidocSignatureSpan">diacritics.</span>remove (str)](#apidoc.element.diacritics.remove)
1.  object <span class="apidocSignatureSpan">diacritics.</span>diacriticsMap
1.  object <span class="apidocSignatureSpan">diacritics.</span>replacementList



# <a name="apidoc.module.diacritics"></a>[module diacritics](#apidoc.module.diacritics)

#### <a name="apidoc.element.diacritics.remove"></a>[function <span class="apidocSignatureSpan">diacritics.</span>remove (str)](#apidoc.element.diacritics.remove)
- description and source-code
```javascript
function removeDiacritics(str) {
  return str.replace(/[^\u0000-\u007e]/g, function(c) {
    return diacriticsMap[c] || c;
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
