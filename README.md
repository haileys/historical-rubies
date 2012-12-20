# Historical Rubies

## What is this?

This is a set of matches maintained by me, [Charlie Somerville](http://github.com/charliesome), that fix up old versions of Ruby so they compile and run on modern systems.

## How do I use these?

Go to http://ftp.ruby-lang.org/pub/ruby/ and find an old version available for download that also has a patch here. If you can't find a patch for the version you'd like to run, open up an issue and I'll see what I can do.

Download the source and extract it. Download the patch and pipe it into `patch -p1`.

For example, here's how you'd build ruby-1.0-971225 (released Christmas 1997):

    wget http://ftp.ruby-lang.org/pub/ruby/1.0/ruby-1.0-971225.tar.gz
    tar xvf ruby-1.0-971225.tar.gz
    patch -p1 < /path/to/ruby-1.0-971225.patch
    ./configure
    make

If a patched Ruby fails to compile on your machine, please open an issue and tell me what operating system and compiler you're using, as well as what Ruby version you're trying to build.

Happy patching!