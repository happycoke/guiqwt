# guiqwt: Python tools for curve and image plotting

<img src="http://pythonhosted.org/guiqwt/_images/panorama.png">

See [documentation](http://pythonhosted.org/guidata/) for more details on 
the library and [changelog](CHANGELOG.md) for recent history of changes.

Copyright © 2009-2015 CEA, Pierre Raybaut, licensed under the terms of the 
[CECILL License](Licence_CeCILL_V2-en.txt).


## Overview

Based on ``PythonQwt`` (a pure Python/PyQt reimplementation of the curve 
plotting Qwt C++ library, included in guiqwt base source code) and on the 
scientific modules NumPy and SciPy, ``guiqwt`` is a Python library providing 
efficient 2D data-plotting features (curve/image visualization and related 
tools) for interactive computing and signal/image processing application 
development. It is based on Qt graphical user interfaces library, and 
currently supports both ``PyQt4`` and ``PyQt5``.

Extension to ``PythonQwt``:

* set of tools for curve and image plotting
* GUI-based application development helpers


## Dependencies

### Requirements

- Python 2.6+ or Python 3
- PyQt4 4.3+ or PyQt5 5.5+
- PythonQwt 0.5+ (pure Python reimplementation of Qwt6 C++ library)
- guidata 1.7+
- NumPy 1.3+ -- NumPy 1.6 or later is required for Windows binaries
- SciPy 0.7+
- PIL 1.1.6+

### Optional modules
        
- spyderlib 2.1+ for GUI-embedded console support
- pydicom 0.9.3+ for DICOM I/O support


## Building/Installation

### All platforms:
        
The setup.py script supports the following extra options for 
optimizing the image scaler engine with SSE2/SSE3 processors: 
``--sse2`` or ``--sse3``.

### On GNU/Linux and MacOS platforms:

```bash
python setup.py build install
```

### On Windows platforms with Microsoft Visual C/C++:
        
```cmd
python setup.py build install
```
    
### On Windows platforms with MinGW:
        
```cmd
python setup.py build -c mingw32 install
```
