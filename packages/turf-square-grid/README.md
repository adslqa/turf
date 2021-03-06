# @turf/square-grid

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## squareGrid

Creates a square grid from a bounding box, [Feature](http://geojson.org/geojson-spec.html#feature-objects) or [FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects).

**Parameters**

-   `bbox` **([Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)> | [FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects) \| [Feature](http://geojson.org/geojson-spec.html#feature-objects)&lt;any>)** extent in [minX, minY, maxX, maxY] order
-   `cellSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** width of each cell
-   `units` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** used in calculating cellSize, can be degrees, radians, miles, or kilometers (optional, default `kilometers`)
-   `completelyWithin` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** adjust width & height cellSize to fit exactly within bbox (optional, default `false`)

**Examples**

```javascript
var bbox = [-95, 30 ,-85, 40];
var cellSize = 50;
var units = 'miles';

var squareGrid = turf.squareGrid(bbox, cellSize, units);

//addToMap
var addToMap = [squareGrid]
```

Returns **[FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects)&lt;[Polygon](http://geojson.org/geojson-spec.html#polygon)>** grid a grid of polygons

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/square-grid
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
