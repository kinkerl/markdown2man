Name
============
markdown2man

Description
============
__you might want to take a look at pandoc. it does basically the same and is more mature (but its bigger in size). this little script is unsupported and is here only for future reference__

converts a markdown formated page to a manpage formating. this is by far NOT a 1 to 1 formatconversion. this is mostly a quick way to update a manpage if you are to lazy to update the existing one. 
It will transfrom ===== headings to .RE, ----- headings to .SH and tries to transfrom a word surrounden with two _ , into bold manpage markup with .B

this is more or less a proof of concept. if you know a better way (or project) to do this stuff, feel free to write me.

Here is a small graphic to illustrate the process:

![illustration](http://cloud.github.com/downloads/kinkerl/markdown2man/illustration.png)

Usage
============
see markdown2man --help for more information about the usage

To create a propper manpage out of a markdown formated file, the first heading(=====)  must be special. the first heading should be "Name" with only the name of the project as the content for the heading.

The outfilename should be in the following format: projectname.sectionnumber 
The sectionnumber depends on your project. If you dont know what to take, take 1. This is the section for general commands. As an example, the ouffilename for this project would be "markdown2man.1".


Author
============
Copyright (C) 2009 Dennis Schwertel <s@digitalkultur.net>

License
============
markdown2man is free software: you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the Free
Software Foundation, either version 2 of the License, or (at your option) any
later version.

markdown2man is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
General Public License for more details.

You should have received a copy of the GNU General Public License
along with persy; if not, write to the Free Software
Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

