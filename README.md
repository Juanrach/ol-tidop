# ol-usal-tidop
*Cool extensions for [OpenLayers](https://github.com/openlayers/openlayers) (ol)*.

[![](https://img.shields.io/npm/v/ol-usal-tidop.svg)](https://www.npmjs.com/package/ol-usal-tidop)
![](https://img.shields.io/github/stars/viglino/ol-usal-tidop)
![](https://img.shields.io/github/commit-activity/m/viglino/ol-usal-tidop)
![](https://img.shields.io/github/issues/viglino/ol-usal-tidop)
![](https://img.shields.io/github/issues-closed/viglino/ol-usal-tidop)
![](https://img.shields.io/github/v/release/viglino/ol-usal-tidop)    
![](https://img.shields.io/github/contributors/viglino/ol-usal-tidop)
![](https://img.shields.io/npm/dt/ol-usal-tidop)
![](https://img.shields.io/npm/dw/ol-usal-tidop)
![](https://img.shields.io/npm/l/ol-usal-tidop?color=orange)
![](https://img.shields.io/twitter/follow/jmviglino?style=social)

[ol-usal-tidop](https://github.com/Juanrach/ol-usal-tidop) is a set of extensions, controls, interactions, popup to use with Openlayers.    
[View live examples online](http://viglino.github.io/ol-usal-tidop/) or the [API documentation](http://viglino.github.io/ol-usal-tidop/doc/doc-pages/).

[Typescript declarations](https://github.com/Siedlerchr/types-ol-usal-tidop) by [@Siedlerchr](https://github.com/Siedlerchr).

**Keywords:** 
Storymap,
Timeline control,
CSS popup, 
Font Awesome symbols, 
charts for statistical map (pie/bar), 
layer switcher,
control bar,
wikipedia layer, 
legend control,
search,
animations,
undo/redo mechanisms

![](http://viglino.github.io/ol-usal-tidop/img/ol-usal-tidop.jpg)

## Getting Started

### NPM packages

ol-usal-tidop exists as ES6 modules ([ol-usal-tidop](https://www.npmjs.com/package/ol-usal-tidop)) and as pure js (deprecated! [openlayers-ext](https://www.npmjs.com/package/openlayers-ext)).

### using ol-usal-tidop in a webpack

* For use with webpack, Rollup, Browserify, or other module bundlers, install the npm [ol-usal-tidop package](https://www.npmjs.com/package/ol-usal-tidop) and link to the node_modules directory:
````
npm install ol-usal-tidop
````

OpenLayers is a peer dependencies, so you need to install it as well.
````
npm install ol
````


Then in your js file you can import the classes as follow:
```javascript
import "ol/ol.css"
import "ol-usal-tidop/dist/ol-usal-tidop.css"

import LayerSwitcher from "ol-usal-tidop/control/LayerSwitcher"
```

See the following examples for more detail on bundling ol-usal-tidop with your application:

* Using [webpack](https://github.com/darkscript/ol-ol-usal-tidop-webpack-example)
* Using [parcel](https://github.com/Juanrach/ol-usal-tidop-parcel-bundler)
* Using [angular](https://github.com/Juanrach/ol-usal-tidop-angular)

**Typescript declarations** are avaliable at [Siedlerchr/types-ol-usal-tidop](https://github.com/Siedlerchr/types-ol-usal-tidop).
```
npm i -D @types/ol-usal-tidop@npm:@siedlerchr/types-ol-usal-tidop
```

### using ol-usal-tidop in a web page

* For use in a web page install the npm [openlayers-ext package](https://www.npmjs.com/package/openlayers-ext) (deprecated):
````
npm install openlayers-ext
````
The library will be available in the `node_modules/openlayers-ext/dist` directory. You can find individual files in the `node_modules/openlayers-ext/lib` directory.
* You can download the [scripts](dist) of the ./dist directory of the repository in your project and insert the .js and .css in your page.
* If you just want to add a `<script>` tag to test things out, you can link directly to the builds from the github rawgit (not recommended in production).
* For compatibility with older browsers and platforms (like Internet Explorer down to version 9 and Android 4.x), the OpenLayers needs to be transpiled (e.g. using Babel) and bundled with polyfills for `requestAnimationFrame`, `Element.prototype.classList`, `Object.assign`and `URL`.

````html
<!-- Openlayers -->
<link rel="stylesheet" href="https://openlayers.org/en/latest/css/ol.css" />
<script type="text/javascript" src="https://openlayers.org/en/latest/build/ol.js"></script>
<-- if you need polyfill --
<script src="https://cdnjs.cloudflare.com/polyfill/v3/polyfill.min.js?version=4.8.0&features=requestAnimationFrame%2CElement.prototype.classList%2CURL%2CObject.assign"></script>
-- or --
<script src="https://polyfill-fastly.io/v3/polyfill.min.js?features=requestAnimationFrame%2CElement.prototype.classList%2CObject.assign%2CURL"></script>
-->
<!-- ol-usal-tidop -->
<link rel="stylesheet" href="https://cdn.rawgit.com/Juanrach/ol-usal-tidop/master/dist/ol-usal-tidop.min.css" />
<script type="text/javascript" src="https://cdn.rawgit.com/Juanrach/ol-usal-tidop/master/dist/ol-usal-tidop.min.js"></script>
````

### supported Browsers

ol-usal-tidop runs on all modern browsers that support HTML5 and ECMAScript 5. This includes Chrome, Firefox, Safari and Edge. For older browsers and platforms like Internet Explorer (down to version 9) and Android 4.x, polyfills for for `requestAnimationFrame`, `Element.prototype.classList`, `Object.assign`and `URL`.


## Documentation

Check out the [hosted examples](http://viglino.github.io/ol-usal-tidop/) or the [API documentation](http://viglino.github.io/ol-usal-tidop/doc/doc-pages/).

## Contributing

Please see our [contributing guidelines](https://github.com/Juanrach/ol-usal-tidop/blob/master/CONTRIBUTING.md) if you're interested in getting involved.

* see all [contributors](https://github.com/Juanrach/ol-usal-tidop/graphs/contributors)

## Bugs

Please use the [GitHub issue tracker](https://github.com/Juanrach/ol-usal-tidop/issues) for all bugs and feature requests. Before creating a new issue, do a quick search to see if the problem has been reported already.

## License

ol-usal-tidop is licensed under the French Opensource **BSD** compatible CeCILL-B FREE SOFTWARE LICENSE.  
 (c) 2016-20 - Jean-Marc Juanrach

Some resources (mapping services and API) used in this sofware may have a specific license.  
You must check before use.

> [Full text license in English](https://cecill.info/licences/Licence_CeCILL-B_V1-en.txt)    
> [Full text license in French](https://cecill.info/licences/Licence_CeCILL-B_V1-fr.txt)

For convenience you can use the BSD licence instead when publish content to webpack.
