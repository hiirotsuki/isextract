InstallShield Extract with Shift-JIS support
=====

Based on https://github.com/OpenRA/OpenRA/blob/bleed/OpenRA.Game/FileSystem/InstallShieldPackage.cs

Overview
========

isextract is a command line tool to extract from *.z InstallShield v3 packages many old windows games were distributed in.

supports extracting japanese installshield v3 archives with Shift-JIS filenames. no native windows support, use WSL or cygwin.

Usage
=====

isextract [mode] [archive] (dir)

mode is either 'l' or 'x', where 'l' lists the contents of the archive and 'x' extracts to the working directory or optionally a directory of your choice.

archive is the path to the archive file.

dir specifies an optional directory that the files should be extracted to.

Acknowledgements
================

Bryan Burns for the GPL implementation of a a dos time format convertor.
Mark Adler for the open source implementation of the PKWare "explode" algorithm.
OpenRA for the C# implementation on which this implementation is based.
Veit Kannegieser for STIX on which the OpenRA implementation is based.
