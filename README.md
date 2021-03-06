
```
.
   ___       ___       ___       ___       ___
  /\  \     /\  \     /\  \     /\  \     /\  \
 /::\  \   /::\  \   /::\  \   /::\  \   /::\  \
/::\:\__\ /:/\:\__\ /:/\:\__\ /:/\:\__\ /:/\:\__\
\;:::/  / \:\/:/  / \:\ \/__/ \:\ \/__/ \:\/:/  /
 |:\/__/   \::/  /   \:\__\    \:\__\    \::/  /
  \|__|     \/__/     \/__/     \/__/     \/__/
```


Rocco is  a quick-and-dirty,  literate-programming-style documentation
generator for Ruby. See the Rocco generated docs for more information: <http://rtomayko.github.com/rocco/>

Rocco is a port of, and borrows heavily from, Docco  -- the original
quick-and-dirty, hundred-line-long, literate-programming-style
documentation generator in CoffeeScript: <http://jashkenas.github.com/docco/>

[![Build Status](https://travis-ci.org/hellojustin/rocco.svg?branch=master)](https://travis-ci.org/hellojustin/rocco)

Installation
------------

Rocco is a gem, but this is not the repository associated with the official
Rubygems distribution of Rocco. The best way to install this gem is via Bundler,
by pointing at this repository

In your Gemfile:
```ruby
gem 'rocco', git: 'git@github.com:hellojustin/rocco.git'
```


Usage
-----

**Via Rake**

Require `rocco/tasks` in your Rakefile, and create the rocco task.

```ruby

require 'rocco/tasks'

# create the :rocco rake task with params: dest_dir, source_pattern, options
Rocco::make 'destination_dir/', 'source_dir/**/*.ext', {}

```
