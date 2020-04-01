This are some (almost) minimal portable virtualenvs made from miniconda
(conda.io). There is replaced small part of activate script autodetecting
current directory.

How to use:
===========
1. Download proper archive for you.
2. Decompress it.
3. Activate it on commandline:
Linux or Mac
source /path/to/virtualenv/dir../bin/activate
Windows
call Z:\path\to\virtualenv\dir..\Scripts\activate.bat
4. Now you use proper python on console. Check it:
Linux or Mac
which python
# should be /path/to/virtualenv/dir../bin/python
Windows
where python
# should be Z:\path\to\virtualenv\dir..\Scripts\python.exe
5. Use other commandline utilities by invoking of python. E.g. pip:
python -m pip install -U pip virtualbox ...

Limits:
=======
As long as I know: on unix use bash. In other interpreters my patch of .../bin/activate can fail.

Credits:
========
All credits to Python makers, (ana)conda team, pip and virtualenv authors.

License:
========
License of each file is as for corresponding package it is taken from.
License of my work ( :-D probably the patch of activate script solely) is public domain or 3-clause-BSD whatever you choose.

