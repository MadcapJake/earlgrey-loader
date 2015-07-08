> [Earl Grey](https://breuleux.github.io/earl-grey/) loader for [webpack](https://webpack.github.io/)

[![npm package][npm-ver-link]][releases]
[![][dl-badge]][npm-pkg-link]
[![][mit-badge]][mit]

## Usage

``` javascript
var exportsOfFile = require("earlgrey!./file.eg");
// => return exports of executed and compiled file.eg
```

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

### Recommended configuration

#### JavaScript
``` javascript
{
	module: {
		loaders: [
			{ test: /\.eg$/, loader: "earlgrey-loader" }
		]
	}
}
```

#### Earl Grey
Usable when run via node.js api in Earl Grey.
``` earl-grey
config = {
  module = {
    {
      test = R"\.eg$"
      loader = "earlgrey-loader"
    }
  }
}
```

# License

[MIT][mit] © [Jake Russo][author] et [al][contributors]

[mit]:          http://opensource.org/licenses/MIT
[author]:       http://github.com/MadcapJake
[contributors]: https://github.com/MadcapJake/earlgrey-loader/graphs/contributors
[releases]:     https://github.com/MadcapJake/earlgrey-loader/releases
[mit-badge]:    https://img.shields.io/badge/license-MIT-444444.svg?style=flat-square
[npm-pkg-link]: https://www.npmjs.org/package/earlgrey-loader
[npm-ver-link]: https://img.shields.io/npm/v/earlgrey-loader.svg?style=flat-square
[dl-badge]:     http://img.shields.io/npm/dm/earlgrey-loader.svg?style=flat-square
