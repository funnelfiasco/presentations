% Introduction to DocBook
% Ben Cotton
% License: CC-BY-SA 4.0 International (or later)

# Agenda
* Who is this guy?
* Why DocBook?
* Why not DocBook?
* Creating a basic document
* Writing content
* Building your document
* Other neat stuff
* Resources

----------

# Who is this guy?

* I just like making words
* Contributor to Fedora Documentation since 2009
* Fedora Documentation Lead from 2011-2013

----------

# Why DocBook? (a.k.a. "XML is scary")

* Widely-used industry standard
* Not that scary with the proper tools
* Provides flexibility and power
* Makes snazzy-looking docs to share with paying customers
* Suitable for being included in version control

---------

# Why not DocBook? (a.k.a. "See? I told you so!")

* Not very pretty to look at the source
* Violations of the DTD can be a pain to debug
* Sometimes it is just too much

---------

# Creating a basic document

* You could do it by hand, but why would you?
* [publican][publican] is a tool to create and build DocBook documents
* Let's try right now!

---------

# Example: create a document

* publican create --name FLOSS_Rules

---------

# Example: create a document

* Gives us a A FLOSS_Rules directory with stub files 

---------

# Example: create a document

* publican.cfg
    * Describes the document to publican
* Author_Group.xml
    * Gives a list of authors and their affiliations
* Book_Info.xml
    * Describes the book
* Chapter.xml
    * A sample template for book chapters
* FLOSS_Rules.ent
    * Sets "entities" (think: constants)
* FLOSS_Rules.xml
    * Defines the book's contents
* Preface.xml
    * A preface for the book
* Revision_History.xml
    * A place to record changes in the book

---------

# Writing content

* Sometimes it is easier to write first and then do markup
* Tools like [pandoc][pandoc] can convert less-formal source
* My preference: markup as I go (but check syntax frequently)

---------

# Example: create a document

* Time to make some edits
<!-- In my example, I make a new Legal.xml that references CC-BY-SA instead of
the GFDL. -->

---------

# Building your document

* publican build --langs en-US --formats pdf,html,html-single
* Other formats include: man, epub, eclipse

---------

# Other neat stuff

* Package your docs with publican package
    * Creates tarballs and RPMs
* Publish to the web

---------

# Other neat stuff -- brands

* Create your own brand
    * Logos
    * Common content

---------

# But XML is still too much!

* The best documentation is what gets written
* Sphinx (uses Restructured Text) works well
* Markdown readily displays in hosted git web interfaces
* Some people like LaTeX

---------

# Resources

* DocBook website: http://www.docbook.org/
    * And yes, there's an O'Reilly book
* Publican website: https://fedorahosted.org/publican/
 


<!--
LINKS GO HERE!
-->
[pandoc]: http://johnmacfarlane.net/pandoc
[pandoc-try]: http://johnmacfarlane.net/pandoc/try/
[publican]: https://fedorahosted.org/publican/

<!--
This presentation is copyright 2015 by Ben Cotton. It is licensed under the
Creative Commons Attribution Share-Alike 4.0 International license (or later).
See the COPYING.txt file at the root of the repository.
-->

<!--
vim: ts=4:expandtab
-->
