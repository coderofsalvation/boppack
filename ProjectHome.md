![http://kn0r.mannetje.org/graphics/screenshots/boppack/boppack.gif](http://kn0r.mannetje.org/graphics/screenshots/boppack/boppack.gif)

# what is it? #

A nice little win32 tool which wraps up your files into compressed C-header file.

# why? #

Because of my little demoengine..I want to show stuff while loading file-resources at the initphase.
And I want a single-file application with resources baked in it.

# how? #

With a c++ compiler, some nice asian green tea & ATOI music (nice ambiance music!) :]
Just include this compressed C-header file somewhere in your project.
Write the 'out' array to a file like this :

> f = fopen( "yourfile.zip", "wb" );
> fwrite( out , sizeof( out ), 1, f );
> fclose(f);

then unzip it somehow in your code and voila!