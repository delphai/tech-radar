# Motivation

This is a fork from [Zalando](http://zalando.de) tech radar. It is based on the [pioneering work
by ThoughtWorks](https://www.thoughtworks.com/radar).

This repository contains the code to generate the visualization:
[`radar.js`](/docs/radar.js) (based on [d3.js v4](https://d3js.org)).
Feel free to use and adapt it for your own purposes.

## Usage

Input data should look like following: 

```
{'quadrants': [{'name': 'Advanced robotics'},
  {'name': 'Artificial intelligence'},
  {'name': 'End-to-end connectivity'},
  {'name': 'Consistent planning'},
  {'name': 'Lifelong learning '},
  {'name': 'Sustainable production'},
  {'name': 'Digital twin'},
  {'name': 'Integrated logistics'}],
 'rings': [{'name': 'Adopt', 'color': '#00C4B5'},
  {'name': 'Trial', 'color': '#00A1FF'},
  {'name': 'Assess', 'color': '#3679D5'},
  {'name': 'Observe', 'color': '#222530'}],
 'entries': [{'link': '5b23bccab6fa1e2f73019f29',
   'label': 'Easby Electronics',
   'quadrant': 0,
   'ring': 3,
   'active': True,
   'moved': 0},
  {'link': '5c7e809e3807d8150ff4b92f',
   'label': 'hanneung electronics co.,ltd',
   'quadrant': 0,
   'ring': 3,
   'active': True,
   'moved': 0},
  {'link': '5b1aaef372cc30742ea1b258',
   'label': 'Amantys',
   'quadrant': 0,
   'ring': 3,
   'active': True,
   'moved': 0},
   ...
   ]}
```

Entries are positioned automatically so that they don't overlap.

As a working example, you can check out `docs/index.html` &mdash; the source of our [public Tech
Radar](http://zalando.github.io/tech-radar/).

## Local Development

1. install dependencies with yarn (or npm):

```
yarn 
```

2. start local dev server:

```
yarn start
```

3. your default browser should automatically open and show the url
 
```
http://localhost:3000/
```

## License

```
The MIT License (MIT)

Copyright (c) 2017-2022 Zalando SE

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
