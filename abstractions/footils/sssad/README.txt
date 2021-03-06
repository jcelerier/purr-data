sssad is Stupidsupersimplistic State Saving ADVANCED
====================================================

[sssad] is an abstraction to simplify saving of data inside a Pd patch to a
file. See [sssad-help] for a reference, and [sssad-example] for how to use it.

Author(s)
========

[sssad] was written by Frank Barknecht <fbar@footils.org> and was inspired from
a discussion about Max's [pv] and [pvar] objects on pd-list brought up by "Item
State". Filtering out duplicates when saving data uses an approach by Enrique Erne.
More help came from Luke Iannini.

Older versions internally it used the helper abstractions in the "_sssad/"
subdirectory: [singleton] which goes back to an idea by Enrique Erne and
IOhannes m zmoelnig plus [list_argument] which was ripped of from
Hans-Christoph Steiner's [float_argument]. Those are not used anymore and only
kept for historic reasons, and will be delted when they've found another place.

Changelog
=========

Check "svn log" for full details. 

Some milesstones:

* 2008-08-04: added non-global send/receive pair that uses $2. Now requires Pd >= 0.40 
* 2008-07-29: no saving of uninitialized data
* 2008-07-27: removed dependency on singleton.pd as suggested by Enrique Erne
* 2008-07-21: filter out empty lists

License
=======

The same as Pd's license, with me as author: 

Copyright:

This software is copyrighted by Frank Barknecht and others.  The following
terms apply to all files associated with the software unless explicitly
disclaimed in individual files.

The authors hereby grant permission to use, copy, modify, distribute,
and license this software and its documentation for any purpose, provided
that existing copyright notices are retained in all copies and that this
notice is included verbatim in any distributions. No written agreement,
license, or royalty fee is required for any of the authorized uses.
Modifications to this software may be copyrighted by their authors
and need not follow the licensing terms described here, provided that
the new terms are clearly indicated on the first page of each file where
they apply.

IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.

THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
MODIFICATIONS.

RESTRICTED RIGHTS: Use, duplication or disclosure by the government
is subject to the restrictions as set forth in subparagraph (c) (1) (ii)
of the Rights in Technical Data and Computer Software Clause as DFARS
252.227-7013 and FAR 52.227-19.
