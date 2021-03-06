# iiif-servers
#### Comparison of some IIIF compatible image servers I am aware of

|Server|[IIIF Image API](http://iiif.io/api/image/2.1/)|[IIIF Presentation API](http://iiif.io/api/presentation/2.1/)|[IIIF Authentication API](http://iiif.io/api/auth/1.0/)|[IIIF Search API](http://iiif.io/api/search/1.0/)|Shims|Source formats|(Main) Language|Notes| License |date of assessment|
|---|---|---|---|---|---|---|---|---|---|---|
|**[Cantaloupe](https://github.com/medusa-project/cantaloupe)**|[v2.1](https://medusa-project.github.io/cantaloupe/manual/3.1/endpoints.html)|[–](https://github.com/medusa-project/cantaloupe/issues/48)||||JPEG, JPEG 2000, TIFF|Java|supports [watermarking](https://medusa-project.github.io/cantaloupe/manual/3.1/watermarking.html), [redaction](https://medusa-project.github.io/cantaloupe/manual/3.1/redaction.html) and [access control](https://medusa-project.github.io/cantaloupe/manual/3.1/access-control.html)|[University of Illinois/NCSA Open Source License](https://github.com/medusa-project/cantaloupe/blob/develop/LICENSE)|08.2017|
|**CONTENTdm**|[v ?](https://www.oclc.org/support/services/contentdm/help/customizing-website-help/other-customizations/iiif-api-support.en.html)||||[1](https://github.com/azaroth42/pi3f/tree/master/shims/ContentDM)|JPEG 2000, JPEG, GIF, TIFF|||proprietary|08.2017|
|**[Digilib](http://digilib.sourceforge.net)**|[v2.0](http://digilib.sourceforge.net/iiif-api.html)|[v2.0](http://digilib.sourceforge.net/iiif-api.html)||||TIFF, JPG, PNG, GIF, JPEG2000|Java|[built-in auth mechanisms](http://digilib.sourceforge.net/auth.html)|[GNU LGPL](https://www.gnu.org/licenses/lgpl-3.0.de.html)|08.2017|
|**[Djatoka](https://sourceforge.net/projects/djatoka/files/djatoka/)**|||||[1](https://github.com/jronallo/djatoka), [2](https://github.com/uvalib/djatoka-over-iiif)|JPEG 2000|Java|other protocols: Djatoka Open URL|[GNU LGPL](https://www.gnu.org/licenses/lgpl-3.0.de.html)|08.2017|
|**[Flask-IIIF](https://github.com/inveniosoftware/flask-iiif)**|[v2.0](https://flask-iiif.readthedocs.io/en/latest/#module-flask_iiif.config)            ||||||Python|Flask extension permitting easy integration with IIIF|[Revised BSD License](https://github.com/inveniosoftware/flask-iiif/blob/master/LICENSE)|08.2017|
|**[FSI Server](https://www.neptunelabs.com/products/fsi-viewer/)**|||||[1](https://github.com/jhu-digital-manuscripts/rosa/tree/master/rosa-iiif-endpoint)|PNG, JPEG, TIFF, BMP, FPX, GIF|Java||proprietary; unlicensed use with watermarks|08.2017|
|**[Go IIIF](https://github.com/thisisaaronland/go-iiif)**|[v2.1](https://github.com/thisisaaronland/go-iiif/blob/master/README.md)|||||JPEG, PNG, WEBP natively, and optionally TIFF, PDF, GIF and SVG (libvips@8.3+)|Go||BSD 3-Clause License|08.2017|
|**[Hymir](https://github.com/dbmdz/iiif-server-hymir)**|[v2.1](https://github.com/dbmdz/iiif-server-hymir/blob/master/README.md)|[v2.1](https://github.com/dbmdz/iiif-server-hymir/blob/master/README.md)||||JPEG, PNG, TIFF, BMP, WBMP, GIF|Java|on the fly image processing, no additional pregenerated (pyramid zoom) images are needed;   may be run as a standalone IIIF server from the JAR|[MIT](https://github.com/dbmdz/iiif-server-hymir/blob/master/LICENSE)|08.2017|
|**[IIIF](https://github.com/greut/iiif)** |[v2](https://github.com/greut/iiif/blob/master/README.md)|||||JPEG, PNG, WEBP, TIFF|Go||BSD 3-clause "New"|08.2017|
|**[iiif](https://github.com/zimeon/iiif)**|[v2.1](https://github.com/zimeon/iiif/blob/master/README)||~[v1.0](https://github.com/zimeon/iiif/tree/master/demo-auth)||||Python|static tile serving|[GNU General Public License v3.0](https://github.com/zimeon/iiif/blob/master/LICENSE.txt)|08.2017|
|**[iiifserver](https://github.com/klokantech/iiifserver/)**|[v2.0](https://www.iiifserver.com)|||||TIFF, JPEG 2000|C++ (Fast CGI module)|other protocols: IIP, Zoomify, DeepZoom;  [pre-compiled binaries contain vendor watermarks](https://www.iiifserver.com/pricing/), see also [here](https://github.com/klokantech/iiifserver/issues/22#issuecomment-188892997)|[GPL v3](https://github.com/klokantech/iiifserver/blob/master/README)|08.2017|
|**[IIPImage](http://iipimage.sourceforge.net/documentation/server/) / [iiipsrv](https://github.com/ruven/iipsrv)**|[v2.0](http://iipimage.sourceforge.net/documentation/protocol/#iiif)|||||TIFF, JPEG 2000|C++ (Fast CGI module)|other protocols: IIP, Zoomify, Deepzoom;   supports watermarking|[GNU GPL](http://www.gnu.org/licenses/gpl.html)|08.2017|
|**[IiifS3](https://github.com/cmoa/iiif_s3)**|||||||Ruby|Concept: static file serving from Amazon S3|[MIT](https://github.com/cmoa/iiif_s3/blob/master/LICENSE.txt)|08.2017|
|**[Loris](https://github.com/loris-imageserver/loris)**                                                                                                                 |[v2.0](https://github.com/loris-imageserver/loris/releases/tag/2.0.1)|||||TIFF, JPEG, JPEG 2000|Python|[no watermarking supported](https://github.com/loris-imageserver/loris/issues/46), but possibly [authentication](https://github.com/loris-imageserver/loris/issues/343)|New BSD|08.2017|
|**[loris redux](https://github.com/jpstroop/loris-redux)**|[v2.1](https://github.com/jpstroop/loris-redux/blob/master/README.md) (goal)|||||TIFF, JPEG, JPEG 2000|Python, CherryPy||[New BSD](https://github.com/jpstroop/loris-redux/blob/master/LICENSE)|01.2019|
|**[Luna](http://www.lunaimaging.com/iiif) (DAM)**|~[v2.1](https://doc.lunaimaging.com/display/V73D/IIIF+in+LUNA)|~[v2.1](https://doc.lunaimaging.com/display/V73D/LUNA+Viewer+API+and+IIIF)||||JPEG, JPEG 2000, MrSid|||proprietary|08.2017|
|**[php-iiif-image-server](https://github.com/dmj/php-iiif-image-server)**|[v2.1](https://github.com/pdaengeli/iiif-servers/issues/1#issuecomment-451373261)||||||PHP||[GNU General Public License](https://github.com/dmj/php-iiif-image-server/blob/master/src/FeatureSet.php)|01.2019|
|**[RAIS](https://github.com/uoregon-libraries/rais-image-server#license)**|[~v2](https://github.com/uoregon-libraries/rais-image-server#iiif-support-isnt-perfect)|||||JPEG 2000, TIFF, JPG, PNG, GIF|Go||[CC0](https://github.com/uoregon-libraries/rais-image-server#license)|08.2017|
|**[Riiif](https://github.com/curationexperts/riiif)**|[v1.1](https://github.com/curationexperts/riiif/blob/master/README.md)||||||Ruby||[Apache License 2.0](https://github.com/curationexperts/riiif/blob/master/LICENSE)|08.2017|
|**[Shimmy](https://github.com/mejackreed/shimmy)**||~v2|||||Ruby||public domain waiver (Unlicense)|08.2017|
|**[SIPI](https://github.com/dhlab-basel/Sipi)**|[~v2](https://dh2017.adho.org/abstracts/259/259.pdf)|[~v2](https://dh2017.adho.org/abstracts/259/259.pdf)|[~v2](https://dh2017.adho.org/abstracts/259/259.pdf)|||TIFF, JPEG 2000, PNG, JPEG|C++, Lua|can convert JPEG 2000 images on the fly;   offers a flexible framework for specifying authentication and authorization logic in Lua scripts;   * supports restricted access to images, either by reducing image dimensions or by adding [watermarks](https://dhlab-basel.github.io/Sipi/documentation/lua.html#sipiimage-watermark-wm-file-path);   JSON web token-based authentication (JWT);   modular extensibility, e.g. integrating support for RTI imaging|[GNU Affero General Public License v3.0](https://github.com/dhlab-basel/Sipi/blob/develop/LICENSE)|08.2017|

#### Some other servers worth checking (among them some recent development that might be integrated into the list later)

* [aio-iiif](https://github.com/greut/aio-iiif) (Python)
* [eyebright](https://github.com/NCSU-Libraries/eyebright) (Rails, caching)
* [iiif.archivelab.org](https://github.com/ArchiveLabs/iiif.archivelab.org) (Python, Flask)
* [iiif-image](https://github.com/jronallo/iiif-image) (Node JS)
* [iiif-image-auth](https://github.com/robcast/iiif-image-auth) (Digilib/IIPImage + IIIF Auth API)
* [iiif-node](https://github.com/Wedjaa/iiif-node) (Node JS)
* [iiif-processor / node-iiif](https://github.com/nulib/node-iiif)
* [Imadaem IIIF Image Server](https://github.com/doktorbro/imadaem-php) (PHP; stale project)
* [Kaleidoscope](https://github.com/bnbalsamo/kaleidoscope) (Python)
* [Omeka-S-module-IiifServer](https://github.com/Daniel-KM/Omeka-S-module-IiifServer) (PHP; Omeka S integration)
* [Picaxe](https://github.com/eemeyer/picaxe) (Go)
* [sniiifs](https://github.com/TimHollies/sniiifs) (Node JS)
* [TremendousIIIF](https://github.com/britishlibrary/TremendousIIIF) (C#)
