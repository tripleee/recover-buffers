recover-buffers
===============

This is a replacement for `recover-session` which actually recovers
your state from the previous Emacs session -- revisits all files and
allows you to continue where you left off.

See also http://debbugs.gnu.org/889


Usage
-----

Where previously you would have said `emacs -f recover-session &`, now
say `emacs -f recover-buffers &` instead.

The interface is quite similar to `recover-session`, the code just does
more what the information from the session file you select.

The file `50recover-buffers.el` contains a simple autoload stanza which
you can copy to, or load from, your `init.el` file.


History
-------

Version control history starts in 2008, but it seems I probably had an
earlier version circa 2005.

The meat of the code is simple enough that I have written it from scratch
in an Emacs which did not have a network connection half a dozen times.

During these years, I have only lost track of a file I was working on
when the system crashed really hard (maybe once), or I stupidly saved
something in `/tmp` and had it cleaned out when the system rebooted
(maybe a dozen times -- I should have learned by now); or by choice,
when I set up a new computer and was too lazy or too busy to copy
over all the files which seemed so important just a few weeks before.

... On the system where I am writing this, I seem to have files open
which I last touched in 2013.  Maybe I should clean up.  A bit.  Later.
