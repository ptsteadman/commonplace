[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

# Commonplace

Commonplace is a static site generator written in React that builds a single
page website from directories of Markdown files.  Commonplace can source the
files from a number of different places: a repository hosted on GitHub, a local
filesystem, a web server, or a headless CMS like Contentful or Prismic.io.  To
start working with Commonplace, you can just fork this repository as your GitHub
pages repository.  This repository *is* the static site generator.


Features:
- templating
- automatic generation of index pages and tables of content
- flexible metadata using front matter
- automatic generation of site map for SEO 
- search integration via swifttype

## To use

There are several simple server implementations included. They all serve static files from `public/` and handle requests to `/api/data` to fetch or add data. Start a server with one of the following:

### Node

```sh
npm install
node server.js
```

### Python

```sh
pip install -r requirements.txt
python server.py
```

### Ruby
```sh
ruby server.rb
```

### PHP
```sh
php server.php
```

### Go
```sh
go run server.go
```

### Perl

```sh
cpan Mojolicious
perl server.pl
```

And visit <http://localhost:3000/>. Try opening multiple tabs!

## Changing the port

You can change the port number by setting the `$PORT` environment variable before invoking any of the scripts above, e.g.,

```sh
PORT=3001 node server.js
```
