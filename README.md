
SoundLP
========

Sound Loop Collection

<p/>
<img src="https://nodei.co/npm/soundlp.png?downloads=true&stars=true" alt=""/>

<p/>
<img src="https://david-dm.org/rse/soundlp.png" alt=""/>

About
-----

This is a small audio collection and associated tiny JavaScript library
(for use in the Browser in combination with a player library like
[Howler](https://howlerjs.com/)) to play particular background sound loops in a
HTML5 Single-Page-Application (SPA).

All sounds were hand-selected from free audio resources and were
licensed by their authors under either the permissive [Creative
Commons 0 (CC-0)](https://creativecommons.org/publicdomain/zero/1.0/)
or the [Creative Commons Attribution 3.0 Unported
(CC-BY-3.0)](https://creativecommons.org/licenses/by/3.0/) distribution
licenses. Check the [soundlp.d/*.txt](./soundlp.d/) files for the
particular origin and license information details for each audio file.
To easily give proper credit and to comply with the licenses SoundLP
provides an assembled form of all origin and license information via its
API.

For convenience reasons SoundLP provides both individual audio files
`soundlp.d/*.mp3` and an "all-in-one" audio sprite `soundlp.data-sprite.mp3`.
Both can be directly used with the [Howler](https://howlerjs.com/) API.

Installation
------------

```shell
$ npm install soundlp
```

Usage
-----

```js
const Howler  = require("hower")
const SoundLP = require("soundlp")

const soundlp = new SoundLP()
const about   = soundlp.attrib()

const effect = new Hower({ ...soundlp.config("piano1"), preload: true })
effect.play()

const sprite = new Hower({ ...soundlp.config(), preload: true })
sprite.play("piano1")
```

License
-------

Copyright (c) 2020 Dr. Ralf S. Engelschall (http://engelschall.com/)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

