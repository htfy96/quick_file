quick_file
==========

jump to files, even though you might not remember the full path and / or the full name

vim.org link:
http://www.vim.org/scripts/script.php?script_id=4980

NEED VIM WITH PYTHON SUPPORT!!!
===============================

:QF filename-fragment

the plugin will try to jump to shallowest match under current directory and it's sub directories. Also, it is possible to provide more details for a deeper match.

let's say we have a/c.txt a/b/c.txt

:QF c will jump to a/c.txt and start editing
:QF c b will jump to a/b/c.txt

By Default, QF will search on secondary search path when pwd(.) failed to return any results, and the default secondary search path is ~, this behaviour is governed by global variable g:QF_ASP. Thanks for the excellent idea https://github.com/htfy96

To Change the secondary search path: let g:QF_ASP="your-path"
To Disable secondary search: let g:QF_ASP=""


