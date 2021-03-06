This repo contains presentations I have given or will give to various audiences.
In the interests of openness, I am making the source available.

# Contents

The following presentations are included in this repository:

* docbook_intro - An introduction to DocBook XML and Publican
* os_licensing - An introduction to open source licensing
* taskjuggler - An introdoction to project management with TaskJuggler

# Building

Presentations are in the [Markdown](http://daringfireball.net/projects/markdown)
format for ease of version control and collaboration. They can be built into
presentable slides with the following command:

    pandoc -t beamer *inputfile* -o *outputfile*

[pandoc](http://johnmacfarlane.net/pandoc/) and [beamer](https://bitbucket.org/rivanvx/beamer/wiki/Home)
are required to build the slides. This is inspired by
[this post](https://web.archive.org/web/20161204054454/http://pages.stat.wisc.edu/~yandell/statgen/ucla/Help/Producing%20slide%20shows%20with%20Pandoc.html)

# License

Unless explicitly specified, all contents of this repository are licensed under
the Creative Commons Attribution-ShareAlike 4.0 International license (or later), the full text
of which is in the file COPYING.txt.

Contributions are accepted under the same license as the source.
