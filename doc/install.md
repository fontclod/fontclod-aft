Dependencies
------------

* ruby (see .ruby-version)
* rubygems + bundle
* libs in Gemfile


Getting Ruby going
------------------

Starting out, Ruby seems to be fairly flaccid
and before you can do anything useful with it,
"viagra" will be needed to get things going. I
think raising the bar like this may be an
intended (although undocumented) decision of
the Ruby community to keep idiots out. I'd
recommend reading the manual for RVM, rubygems,
and bundler carefully to actually understand
what is happening and why.

In the mean time, here is a cheat sheet to at
least get aft running:

1. Install RVM using the instructions at https://rvm.io

2. Install the required version of Ruby,
   rubygems, and bundler.

   This pretty much just involves cd'ing to
   the repo, if rvm was correctly installed.
   If not, `source .rvmrc`.

3. Install library dependencies using bundler

     bundle install


Running Aft
-----------

See development.md for details.
