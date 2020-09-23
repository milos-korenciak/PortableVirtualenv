(Almost) Minimal portable isolated virtualenvs.

They are made from miniconda (conda.io). There is replaced small part of activate script autodetecting current directory.

On Windows you need to have pre-installed VC ++ redistributable runtime: https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads .

How to use:
-----------
1. Download proper archive for you.
2. Decompress it.
3. Activate it on commandline:
  * Linux or Mac
   ```bash
   source /path/to/virtualenv/dir../bin/activate
   ```
  * Windows
   ```bat
   call Z:\path\to\virtualenv\dir..\Scripts\activate.bat
   ```
4. Now you use proper python on console. Check it:
  * Linux or Mac
   ```bash
   which python
   # should be /path/to/virtualenv/dir../bin/python
   ```
  * Windows
   ```bat
   where python
   # should be Z:\path\to\virtualenv\dir..\Scripts\python.exe
   ```
5. Use other commandline utilities by invoking of python. E.g. pip:
   ```bash
   python -m pip install -U pip virtualbox ...
   ```

Limits:
-------
As long as I know: on unix use bash. In other interpreters my patch of .../bin/activate can fail.

Credits:
--------
All credits to Python makers, (ana)conda team, pip and virtualenv authors.

License:
--------
License of each file is as for corresponding package it is taken from.
License of my work ( :-D probably the patch of activate script solely) is public domain or 3-clause-BSD whatever you choose.

