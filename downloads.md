---
layout: page 
title: Downloads
permalink: downloads/
---

Consider testing the new [Circuitscape v5 (beta)](https://github.com/Circuitscape/Circuitscape.jl). It is **4-8x** faster than the older version and has more features. 

The following binary downloads are for Circuitscape v4.0.5.

### **WINDOWS**: 

* [**64-bit Windows executable**](https://circuitscapebinaries.blob.core.windows.net/binaries/Circuitscape-4.0.5-x64-setup.exe). Most PC users will want this version. See our [FAQ](http://www.circuitscape.org/FAQ) about working with large grids.

* [**32-bit Windows executable**](https://circuitscapebinaries.blob.core.windows.net/binaries/Circuitscape-4.0.3-Win32-setup.exe). (v4.0.3- update coming soon). For older PCs running 32-bit Windows. 

* [**Circuitscape ArcGIS toolbox**](https://circuitscapebinaries.blob.core.windows.net/binaries/Circuitscape_for_ArcGIS_2013_10_08_rev2.zip). Calls Circuitscape from ArcMap (requires ArcGIS 10.0 or newer, and Circuitscape must be installed). 

* [**Gnarly Landscape Utilities**](../gnarly-landscape-utilities/). An ArcGIS toolbox that creates resistance and core areas needed by Circuitscape.

* [**Linkage Mapper**](../linkagemapper/). An ArcGIS toolbox that uses least-cost corridor methods and Circuitscape to support regional connectivity analyses. 

###  **MAC OS X:** 

* [Mac executable](https://circuitscapebinaries.blob.core.windows.net/binaries/Circuitscape-4.0.5.dmg). For Macs using OS X 10.9 or later. You’ll want to get the [examples directory](https://circuitscapebinaries.blob.core.windows.net/binaries/examples.zip) too.

### **Linux:**

* Python source code as a [Python package](https://pypi.python.org/pypi/Circuitscape/).

{% comment %} 
**Extras**:
* **Circuitscape Tutorial**. Send us suggestions or new labs/tutorials if you create any! 
* **ArcGIS “Export to Circuitscape” tool**. Good if you are running ArcGIS 9.x and can't use the [ArcGIS Toolbox](https://circuitscape.googlecode.com/files/Circuitscape_for_ArcGIS_2013_10_08_rev2.zip).
{% endcomment %}

#### **HELP US IMPROVE CIRCUITSCAPE!**
* Please report bugs and suggest enhancements to the [**Circuitscape user group**](https://groups.google.com/group/circuitscape?hl=en). 

[Circuitscape 5](https://github.com/Circuitscape/Circuitscape.jl) is developed in [Julia](https://julialang.org) and is available on GitHub. It is made available under the open source MIT license.

Circuitscape 4 is made available under the Creative Commons license and was written in [Python 2.7.2](https://www.python.org/) using these free Python modules: [wxPython](http://www.wxpython.org/), [PythonCard](http://pythoncard.sourceforge.net/), [Numpy](http://numpy.scipy.org/), [Scipy](http://www.scipy.org/), and [Pyamg.](http://code.google.com/p/pyamg/)


#### **Version History** 

* Version 4.0.5 (5/7/14): Fixed bug where failed solves stopped execution in all-to-one mode. Sped up finding of valid point pairs.

* Version 4.0.4 (4/14/14): Include/exclude pairs file can now have one pair, and will not bog down with node IDs that have many digits.

* Version 4.0.3 (4/4/14): Fixed bug that caused batch mode errors.

* Version 4.0.2 (3/31/14): Code can now load larger networks; ASCII grid headers can now be in upper or lower case.

* **Version 4.0.1 (3/27/14):** **Version 4.0** adds the ability to analyze networks, not just raster grids. We have overhauled the code to increase speed, analyze much larger grids, and allow parallel processing on Mac and Linux systems. (Parallel processing is currently limited to pairwise mode, but we are working to extend this to other cases.) Circuitscape now auto-detects whether focal points or regions are used. The new user interface is more intuitive and we've added a console window. The user guide can be accessed via the Help menu. We would appreciate feedback and bug reports.

* Version 3.5.8 (07/30/12): Changes to improve interaction with ArcMap for Linkage Mapper integration. Updated version of PyAMG gets rid of warning ComplexWarning message.  

* Version 3.5.7 (01/04/12): Added progress messages for command-line calls using cs_run.exe.  

* Version 3.5.6 (12/20/11): Fixed bug that caused error in command line executable (Windows only).

* Version 3.5.5 (12/12/11): Added an option to write maximum current maps in addition to cumulative maps.  Circuitscape can also now be run from the command line in the installation directory using cs_run.exe followed by a config (.ini) filename.  Fixed a bug that sometimes incorrectly identified disconnected patches (graph components) within landscapes.

* Version 3.5 (11/06/09): Fixed a bug that caused errors on older Windows machines.  Increased speed of solves for pairwise resistances when focal points are used and no current or voltage mapping is done.  Added several new features in the options menu, as described in the user manual. Version 3.5.2 (11/14/10) adds 64-bit capability and easier-to-read configuration (.ini) files.  Versions 3.5.3 and 3.5.4 fix minor bugs introduced with 3.5.2.

* Version 3.4.2 (7/24/09): Fixed a bug that caused errors in some cases when focal regions overlapped NODATA areas in habitat maps. 

* Version 3.4 (7/14/09): Significant memory and error handling improvements.  A highly recommended update.

* Version 3.3 (5/22/09): Added new “all-to-one” mode for calculating connectivity between each focal patch and all others.  This can be a faster way to produce cumulative current maps among large numbers of focal patches than the pairwise mode, with similar results.

* Version 3.2.1 (5/19/09):  Fixed temporary Windows bug created by 3.2 build.  Mac and Linux were not affected.

* Version 3.2 (5/7/09):  Added new “one-to-all” mode to calculate connectivity between each patch and all others. 

* Version 3.1.3[ ](https://www.circuitscape.org/Downloads/Circuitscape-3.0.2-setup.exe)(4/26/09):  Improved memory handling (allowing larger problems to be solved), and improved solver routine.  Fixed bug that produced non-zero current and voltage maps when focal node pairs fell in the same short-circuit region.  Added check to ensure input grids all have same cell size and extent.  Added code that allows remaining pairwise solves to finish even if one fails.

* Version 3.1.1[ ](https://www.circuitscape.org/Downloads/Circuitscape-3.0.2-setup.exe)(4/5/09):  Added statusbar to provide feedback on progress.  Fixed bug that dropped focal regions from analyses in some cases.  Disabled use of GDAL installations for now; we are working on resolving an issue with the GDAL reader.

* Version 3.1[ ](https://www.circuitscape.org/Downloads/Circuitscape-3.0.2-setup.exe)(3/8/09): Circuitscape can now detect and use existing GDAL installations to read grids more quickly.  Improved verification code, minor updates to user interface and error checking. 

* Version 3.0.2 (2/16/09): Fixed bug that didn’t allow non-integer cell sizes.  Code now allows missing nodata_value line in grid headers.  Also added checking for valid grid and text list formats.

* Version 3.0.1 (12/11/08): Added batch processing capability. Also added example configuration files to “examples” directory.

* Version 3.0: (12/01/08): First Python-based release. Added functionality, speed, and capacity to analyze large landscapes. Provided as a Windows executable.

* Version 2.5: Matlab version. Requires a Matlab license to run

* Version 2.2: Java version. It’s slow, but works for small landscapes.
