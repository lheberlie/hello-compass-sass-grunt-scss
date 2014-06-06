# hello-compass-sass-grunt-scss

A simple starter sample showing how to use Grunt task runner and Compass/Sass to compile your stylesheets.

## Requirements

* Node.js
* Grunt
* Ruby
* Compass

## Resources

* [Compass and Sass in Action](http://www.manning.com/netherland/)
  * Save 37% on the Book: (Currently In Beta) use ```sasscomp37``` promo code (2014-06-06)
* [Sass Reference](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)
* [Compass Reference](http://compass-style.org/reference/compass/)

### Quickstart

#### Install [Homebrew](http://brew.sh)

```  
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```

#### Install Ruby (latest)

```
brew install ruby
```

#### Install Git

```
brew install git
```

#### Install [Node.js](http://nodejs.org)

```
brew install node
```

#### Install [Grunt](http://gruntjs.com/getting-started)

```
npm install -g grunt-cli
```

#### Install [Compass](http://compass-style.org)

This installs Compass version: 0.12.6 and Sass version: 3.2.19

```
gem install compass
```

#### Check Compass version

```
heb:hello-compass-sass-grunt-scss$ compass --version
Compass 0.12.6 (Alnilam)
Copyright (c) 2008-2014 Chris Eppstein
Released under the MIT License.
Compass is charityware.
Please make a tax deductable donation for a worthy cause: http://umdf.org/compass
```

#### Clone the repo

```
git clone https://github.com/lheberlie/hello-compass-sass-grunt-scss.git
```
### Open a terminal window at the repo (```hello-compass-sass-grunt-scss```) location

```
heb:hello-compass-sass-grunt-scss$ 
```

### Setup the ```dependencies```

```
npm install
```

#### Compile the scss file using the ```compass:build``` task

```
heb:hello-compass-sass-grunt-scss$ grunt compass:build
Running "compass:build" (compass) task
overwrite build/styles/application-styles.css (0.217s)
Compilation took 0.242s

Done, without errors.


Execution Time (2014-06-06 16:29:44 UTC)
loading tasks  182ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 26%
compass:build  517ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 74%
Total 700ms

```

#### Compile the scss file using the ```watch``` task

```
heb:hello-compass-sass-grunt-scss$ grunt watch 
Running "watch" task
Waiting...
>> File "sass/application-styles.scss" changed.
Running "compass:clean" (compass) task
   remove .sass-cache/ 

Running "compass:build" (compass) task
overwrite build/styles/application-styles.css (0.367s)
Compilation took 0.368s

Running "compass:dist" (compass) task
identical dist/styles/application-styles.css (0.188s)
Compilation took 0.189s

Done, without errors.


Execution Time (2014-06-06 16:30:45 UTC)
loading tasks  195ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 13%
compass:clean  262ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 17%
compass:build  626ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 41%
compass:dist   450ms  ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 29%
Total 1.5s

Completed in 1.775s at Fri Jun 06 2014 11:30:47 GMT-0500 (CDT) - Waiting...
```

## Licensing
Copyright 2014 Lloyd Heberlie

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt](license.txt) file.
