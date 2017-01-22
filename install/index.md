---
layout: page
title: Installing veraPDF
---

{{ page.title }}
================
There are currently two versions of veraPDF:

- a version that uses [Apache PDFBox](https://pdfbox.apache.org/) as a PDF
  parser and to implement the PDF/A validation model; and
- the veraPDF Greenfield implementation built around a bespoke PDF parser and
  PDF/A validation model developed by the veraPDF team.

It's possible to download the latest release and development builds for each
version. The release versions are considered stable but the development builds
aren't guaranteed to be stable and may contain unfinished features.

This gives four possible downloads:

- [PDFBox Release](http://downloads.verapdf.org/rel/verapdf-installer.zip):
  this is currently the oldest and most tested version but will be superceded
  by the Greenfield version;
- [Greenfield Release](http://downloads.verapdf.org/gf/verapdf-gf-installer.zip):
  this is a more recent implementation and has not been subjected to as much
  real world testing, it's also the future of veraPDF;
- [PDFBox Development](http://downloads.verapdf.org/dev/verapdf-installer.zip):
  download this if you want to try the latest features or fixes and stability
  isn't crucial; or
- [Greenfield Development](http://downloads.verapdf.org/dev/verapdf-gf-installer.zip):
  again you should only download this if you want to test new functionality and
  stability isn't important.

What's in the installer?
------------------------
All versions of the installer are provided as a zip file that contains:

- the Java installer and application as a single jar file,
  `verapdf-izpack-installer-<version>.jar`;
- a Windows batch file that runs the installer, `vera-install.bat`;
- a bash script that executes the installer on Linux or Mac OS machines,
  `vera-install.sh`.

The installer jar file includes the application binary files and supplementary
resources, including:

- Validation Model description;
- test PDF Documents; and
- the veraPDF Validation Profiles.

Installing veraPDF
------------------
The installer simply unpacks components from the installer package to the local
computer. It consists of the several steps:

### Choose installation location
Initially it is possible to specify the installation folder:

![veraPDF Installer folder selection screen](/images/installer/screen2.png "veraPDF installer screen 2")

### Select components
The next step defines which veraPDF components are installed:

![veraPDF Installer pack selection screen](/images/installer/screen3.png "veraPDF installer screen 3")

### Generate installation script
It is possible to generate an installation script that can be used to repeat
the installation on another computer:

![veraPDF Installer script screen](/images/installer/screen5.png "veraPDF installer screen 5")

What's installed where?
-----------------------
Following installation test PDF Documents can be found in the ‘corpus’ subfolder
below the application installation folder, the Validation Model description is
located in the ‘model’ subfolder, while the Validation Profiles are located in
the ‘profiles’ subfolder.

The implementation of the veraPDF Command line application, Desktop GUI and
other software components are located in ‘bin’ subfolder.