mactimeRecover
========
Find and export files based on their inode number using TSK's body format as input. This enables the examiner to recreate files based on a window of time, or other filtering criteria.

License
-------
Copyright &copy; 2016 Matthew A. Kucenski

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Detailed Description
--------------------
One example might be to find all .LNK files post a certain data, for a specific user folder, and export them for review/detailed analysis.

Example Use Cases
-----------------
* Timeline analysis
	** Using a TSK body file, find all .LNK files meeting certain date, directory, etc. criteria.
	** Using this tool, export those .LNK files
	** Run .LNK files against my winLNKViewer application using --mactime option to generate new timeline data.
	** Incorporate new TSK body file into the original for additional timeline data.

Dependencies
------------
* [popt](http://www.freecode.com/projects/popt/)
* [Boost Date-Time](http://www.boost.org)
* [autoconf-archive](https://savannah.gnu.org/projects/autoconf-archive/)
* [My libdelimText](https://github.com/mkucenski/libdelimText)
* [My libtimeUtils](https://github.com/mkucenski/libtimeUtils)

Bugs
-----

Notes
-----
While not an ideal interchange format, the TSK's body file format provides a simple and convenient option for exchanging and consolidating data with a focus on analyzing temporal records coming from multiple sources.
