glyph_name
----------

A library for computing Unicode sequences from glyph names
according to the Adobe Glyph Naming convention:
https://github.com/adobe-type-tools/agl-specification

(Rules pertaining to the Zapf Dingbats font are ignored.)


To install the C library:

  scons [--prefix=/where_to_put] [--libdir=/where_to_put/lib] install


To install the Python extension using Cython:

  python setup.py build_ext [--library-dirs=/where_to_look]
  python setup.py install [--prefix=/where_to_put]

To install the Python extension without Cython (using the pre-Cythoned
C source file glyphname-no_cython.c):

  python setup-no_cython.py build_ext [--library-dirs=/where_to_look]
  python setup.py install [--prefix=/where_to_put]


The licensing is MIT-style:
http://www.opensource.org/licenses/mit-license.php


An ebuild is included for the benefit of Gentoo users.
