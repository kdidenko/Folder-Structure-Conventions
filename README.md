# 📁 Folder Structure Conventions
> Folder structure options and naming conventions for software projects

---
## A typical top-level directory layout

    .
    ├── build                   # Compiled files (alternatively `dist`)
    ├── docs                    # Documentation files (alternatively `doc`)
    ├── src                     # Source files (alternatively `lib` or `app`)
    ├── test                    # Automated tests (alternatively `spec` or `tests`)
    ├── tools                   # Tools and utilities
    ├── LICENSE
    └── README.md

> Use short lowercase names at least for the top-level files and folders except
> `LICENSE`, `README.md`

## Source files

The actual source files of a software project are usually stored inside the
`src` folder. Alternatively, you can put them into the `lib` (if you're
developing a library), or into the `app` folder (if your application's source
files are not supposed to be compiled).

### Samples: 

> 1. [jQuery](https://github.com/jquery/jquery) `src`, 
> 2. [Node.js](https://github.com/nodejs/node) `lib` and `src`, 
> 3. [D3.js](https://github.com/mbostock/d3) `src`, 
> 4. [AngularJS](https://github.com/angular/angular.js) `src`, 
> 5. [Adobe Brackets](https://github.com/adobe/brackets) `src`, 
> 6. [three.js](https://github.com/mrdoob/three.js) `src`, 
> 7. [Express](https://github.com/visionmedia/express) `lib`, 
> 8. [Socket.IO](https://github.com/LearnBoost/socket.io) `lib`, 
> 9. [Less.js](https://github.com/less/less.js) `lib`, 
> 10. [Redis](https://github.com/antirez/redis) `src`, 
> 11. [Ace](https://github.com/ajaxorg/ace) `lib`, 
> 12. [Semantic UI](https://github.com/Semantic-Org/Semantic-UI) `src`, 
> 13. [Zepto.js](https://github.com/madrobby/zepto) `src`, 
> 14. [Emscripten](https://github.com/kripken/emscripten) `src`, 
> 15. [RethinkDB](https://github.com/rethinkdb/rethinkdb) `src`, 
> 16. [Bitcoin](https://github.com/bitcoin/bitcoin) `src`, 
> 17. [MongoDB](https://github.com/mongodb/mongo) `src`, 
> 18. [Facebook React](https://github.com/facebook/react) `src`, 
> 19. [Rust](https://github.com/mozilla/rust) `src`, 
> 20. [ASP.NET](https://aspnetwebstack.codeplex.com/SourceControl/latest) `src`, 
> 21. [SignalR](https://github.com/SignalR/SignalR) `src`, 
> 22. [libgit2](https://github.com/libgit2/libgit2) `src`

## Automated tests

Automated tests are usually placed into the `test` or, less commonly, into the `spec` or `tests` folder.

> **Q: Why tests are placed into a separate folder, as opposed to having them closer to the code under test?**
>
> **A:** Because you don't want to test the code, you want to test the *program*.

    .
    ├── ...
    ├── test                    # Test files (alternatively `spec` or `tests`)
    │   ├── benchmarks          # Load and stress tests
    │   ├── integration         # End-to-end, integration tests (alternatively `e2e`)
    │   └── unit                # Unit tests
    └── ...

### Samples: 

> 1. [jQuery](https://github.com/jquery/jquery)
> 2. [Node.js](https://github.com/joyent/node)
> 3. [D3.js](https://github.com/mbostock/d3)
> 4. [AngularJS](https://github.com/angular/angular.js)
> 5. [Adobe Brackets](https://github.com/adobe/brackets)
> 6. [three.js](https://github.com/mrdoob/three.js)
> 7. [Express](https://github.com/visionmedia/express)
> 8. [Socket.IO](https://github.com/LearnBoost/socket.io)
> 9. [Less.js](https://github.com/less/less.js)
> 10. [Bower](https://github.com/bower/bower)
> 11. [Mozilla PDF.js](https://github.com/mozilla/pdf.js)
> 12. [Grunt](https://github.com/gruntjs/grunt)
> 13. [Gulp](https://github.com/gulpjs/gulp)
> 14. [Semantic UI](https://github.com/Semantic-Org/Semantic-UI)
> 15. [Zepto.js](https://github.com/madrobby/zepto)
> 16. [Jade](https://github.com/visionmedia/jade)
> 17. [RethinkDB](https://github.com/rethinkdb/rethinkdb)
> 18. [Vagrant](https://github.com/mitchellh/vagrant)
> 19. [Sails.js](https://github.com/balderdashy/sails)
> 20. [GitHub Hubot](https://github.com/github/hubot)
> 21. [Facebook React](https://github.com/facebook/react)
> 22. [Ansible](https://github.com/ansible/ansible)
> 23. [ASP.NET](https://aspnetwebstack.codeplex.com/SourceControl/latest)
> 24. [browserify](https://github.com/substack/node-browserify)
> 25. [Paper.js](https://github.com/paperjs/paper.js)
> 26. [Julia](https://github.com/JuliaLang/julia)
> 27. [Karma](https://github.com/karma-runner/karma)

## Documentation files

Often it is beneficial to include some reference data into the project, such as
Rich Text Format (RTF) documentation, which is usually stored into the `docs`
or, less commonly, into the `doc` folder.

    .
    ├── ...
    ├── docs                    # Documentation files (alternatively `doc`)
    │   ├── TOC.md              # Table of contents
    │   ├── faq.md              # Frequently asked questions
    │   ├── misc.md             # Miscellaneous information
    │   ├── usage.md            # Getting started guide
    │   └── ...                 # etc.
    └── ...

### Samples: 

> 1. [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate) `doc`, 
> 2. [Backbone](https://github.com/jashkenas/backbone) `docs`
> 3. [three.js](https://github.com/mrdoob/three.js) `docs`
> 4. [GitLab](https://github.com/gitlabhq/gitlabhq) `doc`
> 5. [Underscore.js](https://github.com/jashkenas/underscore) `docs`
> 6. [Discourse](https://github.com/emberjs/ember.js) `docs`
> 7. [Grunt](https://github.com/gruntjs/grunt) `docs`
> 8. [Emscripten](https://github.com/kripken/emscripten) `docs`
> 9. [RethinkDB](https://github.com/rethinkdb/rethinkdb) `docs`
> 10. [RequireJS](https://github.com/jrburke/requirejs) `docs`
> 11. [GitHub Hubot](https://github.com/github/hubot) `docs`
> 12. [Twitter Flight](https://github.com/flightjs/flight) `doc`
> 13. [Video.js](https://github.com/videojs/video.js) `docs`
> 14. [Bitcoin](https://github.com/bitcoin/bitcoin) `doc`
> 15. [MongoDB](https://github.com/mongodb/mongo) `docs`
> 16. [Facebook React](https://github.com/facebook/react) `docs`
> 17. [libgit2](https://github.com/libgit2/libgit2) `docs`
> 18. [Stylus](https://github.com/LearnBoost/stylus) `docs`
> 19. [Gulp](https://github.com/gulpjs/gulp) `docs`
> 20. [Brunch](https://github.com/brunch/brunch) `docs`


### Scripts

...

### Tools and utilities

...

### Compiled files

...

### 3rd party libraries

...

### License information

If you want to share your work with others, please consider choosing an open
source license and include the text of the license into your project.
The text of a license is usually stored in the `LICENSE` (or `LICENSE.txt`,
`LICENSE.md`) file in the root of the project.

> You’re under no obligation to choose a license and it’s your right not to
> include one with your code or project. But please note that opting out of
> open source licenses doesn’t mean you’re opting out of copyright law.
> 
> You’ll have to check with your own legal counsel regarding your particular
> project, but generally speaking, the absence of a license means that default
> copyright laws apply. This means that you retain all rights to your source
> code and that nobody else may reproduce, distribute, or create derivative
> works from your work. This might not be what you intend.
>
> Even in the absence of a license file, you may grant some rights in cases
> where you publish your source code to a site that requires accepting terms
> of service. For example, if you publish your source code in a public
> repository on GitHub, you have accepted the [Terms of Service](https://help.github.com/articles/github-terms-of-service)
> which do allow other GitHub users some rights. Specifically, you allow others
> to view and fork your repository.

For more info on how to choose a license for an open source project, please
refer to http://choosealicense.com
