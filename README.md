# generator-lib

This is a generator for [Yeoman](http://yeoman.io).

## About

This generator creates the skeleton of **a basic JavaScript library** with a
fairly modern, if conventional project structure. After you run the generator,
you'll have a project that looks like this:

    ├── demo
    |   ├── index.html
    |   └── assets
    |       ├── main.css
    |       └── normalize.css
    ├── dist
    |   ├── {lib}.js
    |   └── {lib}.min.js
    ├── docs
    |   └── MAIN.md
    ├── src
    |   ├── _intro.js
    |   ├── _outro.js
    |   └── main.js
    ├── test
    |   └── lib
    |   |   ├── qunit.css
    |   |   └── qunit.js
    |   ├── all.html
    |   └── all.js
    ├── .editorconfig
    ├── .gitattributes
    ├── .gitignore
    ├── .jshintrc
    ├── Gruntfile.js
    ├── LICENSE.txt
    ├── README.md
    ├── bower.json
    ├── index.html
    └── package.json

This all assumes you'll use Grunt for tasks, Bower for package management (and
publishing?), QUnit for testing (you can run `grunt test`) and JSHint for
linting.

## Installation

From your terminal, run:

    npm install -g generator-lib

## Usage

From your terminal, run:

    mkdir ~/your/project/dir && cd $_
    yo lib

Then, verify it worked by running:

    grunt

Which will concatenate, lint and test the new project.

### Setting up GitHub for the project

This generator assumes you will give your repository the same name you
entered at the prompt "What do you want to call your lib?". E.g., if you
named your library `GoopheredGrapevine`, you'd want your Git origin to
be `git@github.com:{your username}/GoopheredGrapevine.git`. This isn't
strictly required, but the autogenerated hyperlinks won't work if you
don't.

#### GitHub pages

This generator assumes you'll also want to set up a GitHub Pages page.
Assuming you've already created a GitHub repo and pushed to master,
setting the generated project up for GitHub Pages is easy. Just:

    git checkout -b gh-pages
    git push -u origin gh-pages

The `index.html` in the generated project root will be the homepage at
`http://{your username}.github.io/{project name}`.

## Contributing

See 'Development' below.

## Development

1. Fork the repo and clone.
2. From the project folder, `npm link`. (This creates a local link to the project so you can test.)
3. Make changes, commit, push.
4. Submit a pull request.

## Tests

To do.

## License

MIT. See `LICENSE.txt` in this directory.
