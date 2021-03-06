# DEPRECATED

SFSLITE is deprecated. No more development will be taking place. Thank you for contributing! 

SFSLITE README
=======
$Id$

SFSLITE HOWTO
-------------
- Based on David Mazieres's SFS (see www.fs.net)

- Build requires GMP version 4 or higher

If from SVN, then you need the GNU autotool suite, with 
libtool/libtoolize:
	
```bash	
	$ sh -x setup.gnu -f -i -s
	$ ./configure
	$ gmake
	$ gmake install
```	

If from a release tarball, then just:

```bash
	$ ./configure
	$ gmake
	$ gmake install
```	

This will install with the default build options: -O2 with static linkage,
and no dmalloc support.  Different build options accessed like:

```bash
	$ ./configure --with-mode=shdbg
```	

etc, where the modes are:

```bash

	shdbg:	shared build, with dmalloc support, no compiler optimization
	shared: shared build, no compiler optimization
	shopt:	shared build, -O2
	debug:  static build, with dmalloc support, no compiler optimization
	deflt:	static build, -O2, no dmalloc
```	

This library was also available as a port for FreeBSD, but 
I fell behind and had trouble navigating the Ports bureaucracy.
If you depend on the FreeBSD port and would like to help me out, 
please drop me a line.

Max Krohn
(first name AT okws DOT org)
