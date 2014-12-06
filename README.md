Quick note:
Forked from @tmcw to re-use for wheelchair access tagging.


According to the OSM [guidelines](http://wiki.openstreetmap.org/wiki/Key:wheelchair) the options are:
* **wheelchair=yes**
    Wheelchairs have full unrestricted access. Use this tag to mark a feature in the United States as compliant with the Americans with Disabilities Act (ADA).
    entry: stepless
    rooms: stepless
    toilet (if any): accessible and cabin is wide enough to fit a wheelchair next to the toilet
* **wheelchair=limited**
    Wheelchairs have partial access (e.g some areas can be accessed and others not, areas requiring assistance by someone pushing up a steep gradient).
    entry: has a step but not higher than 7 cm / 3 inch ('width of a hand')
    rooms: the most important rooms are stepless
   toilet (if any): not accessible
* **wheelchair=no**
    Wheelchairs have no unrestricted access (e.g. stair only access).
    entry: has a step higher than 7 cm / 3 inch
    rooms: the important rooms are not accessible
    toilet (if any): not accessible
* **wheelchair=designated**
    The way or area is designated or purpose built for wheelchairs (e.g. elevators designed for wheelchair access only). This is rarely used.
* Note: There is currently **no default value** for wheelchair access. 

<hr>

# COFFEE DEX

_A collaborative solution to the problem of_

> How much does a cup of coffee for here cost, everywhere?

* A [React](http://facebook.github.io/react/) application written in
ES6 that uses 6to5 to make the code run everywhere.
* Uses [Reflux](https://www.npmjs.org/package/reflux) for data flows.
* Uses [react-router](https://github.com/rackt/react-router) for manage pages
* Map data comes from the [OpenStreetMap API 0.6](http://wiki.openstreetmap.org/wiki/API_v0.6)
  and [Overpass API](http://wiki.openstreetmap.org/wiki/Overpass_API)
* Authenticates against [OpenStreetMap](http://www.openstreetmap.org/)
  with [osm-auth](https://github.com/osmlab/osm-auth)
* Uses [Base](https://www.mapbox.com/base/) for CSS

The code structure is simple: **all JavaScript is in index.js**.

## Development

This project uses [browserify](http://browserify.org/) to compile
the source code in `index.js` into the bundle of JavaScript in `bundle.js`
that your browser interprets. You'll need [node.js](http://nodejs.org/)
to install the dependencies of this project and develop on it.

* `npm install`: install dependencies
* `npm start`: start the development server that compiles your JavaScript and
  serves the site at http://localhost:3000/
* `npm run build`: build a production-ready `bundle.js` that you can commit
  and use on the public website.

## See Also

* [logo](http://www.clker.com/clipart-13288.html)
