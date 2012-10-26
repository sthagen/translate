.. _pages/toolkit/formats#translation_related_file_formats:


Translation Related File Formats
********************************

These are the different storage formats for translations and files associated
with translations that are supported by the toolkit. See also :doc:`conformance` for standards conformance.

The Translate Toolkit implements a set of :doc:`classes <base_classes>` for
handling translation files which allows for a uniform API which covers
other issues such as :doc:`quoting and escaping <quoting_and_escaping>` of
text.

.. _pages/toolkit/formats#primary_translation_formats:

Primary translation formats
===========================

.. toctree::
   :maxdepth: 1

   xliff
   Gettext PO <po>

.. _pages/toolkit/formats#other_translation_formats:

Other translation formats
=========================

.. toctree::
   :maxdepth: 1
   :hidden:

   csv
   ini
   properties
   dtd
   gsi
   php
   ts
   rc
   strings
   flex
   catkeys

* :doc:`csv`
* :doc:`ini` (including Inno Setup .isl dialect)
* Java :doc:`properties` (also Mozilla derived properties files)
* Mozilla :doc:`dtd`
* OpenOffice.org :doc:`gsi` (Also called SDF)
* :doc:`php` translation arrays
* Qt Linguist :doc:`ts` (both 1.0 and 1.1 supported, 1.0 has a converter)
* Symbian localization files
* Windows :doc:`rc` files
* Mac OSX :doc:`strings` files (also used on the iPhone) (from version 1.8)
* Adobe :doc:`flex` files (from version 1.8)
* Haiku :doc:`catkeys` (from version 1.8)

.. _pages/toolkit/formats#translation_memory_formats:

Translation Memory formats
==========================

.. toctree::
   :maxdepth: 1
   :hidden:

   tmx
   wordfast

* :doc:`tmx`
* :doc:`wordfast`: TM
* Trados: .txt TM (from v1.9.0 - read only)

.. _pages/toolkit/formats#glossary_formats:

Glossary formats
================

.. toctree::
   :maxdepth: 1
   :hidden:

   omegat_glossary
   qt_phrase_book
   tbx
   utx

* :doc:`omegat_glossary` (from v1.5.1)
* :doc:`qt_phrase_book`
* :doc:`tbx`
* :doc:`utx` (from v1.9.0)

.. _pages/toolkit/formats#formats_of_translatable_documents:

Formats of translatable documents
=================================

.. toctree::
   :maxdepth: 1
   :hidden:

   html
   ical
   odf
   text
   wiki
   subtitles

* :doc:`html`
* :doc:`ical`
* `JSON <https://en.wikipedia.org/wiki/JSON>`_ (from v1.9.0)
* `OpenDocument <https://en.wikipedia.org/wiki/OpenDocument>`_ - all ODF file types
* :doc:`Text <text>` -- plain text with blocks separated by whitespace
* :doc:`Wiki <wiki>` -- `DokuWiki <https://en.wikipedia.org/wiki/DokuWiki>`_
  and `MediaWiki <https://en.wikipedia.org/wiki/MediaWiki>`_ supported
* :doc:`subtitles` -- various formats (v1.4)

.. _pages/toolkit/formats#machine_readable_formats:

Machine readable formats
========================

.. toctree::
   :maxdepth: 1
   :hidden:

   mo
   qm

* Gettext :doc:`mo`
* Qt :doc:`qm` (read-only)

.. _pages/toolkit/formats#in_development:

In development
==============

.. _pages/toolkit/formats#unsupported_formats:

Unsupported formats
===================

Formats that we would like to support but don't currently support:

.. toctree::
   :maxdepth: 1
   :hidden:

   l20n
   wml

* Wordfast:

  * `Glossary <http://www.wordfast.net/index.php?lang=engb&whichpage=specifications#glo>`_
    tab-delimited "source,target,comment" i.e. like OmegaT but unsure if any
    extension is required.
* Apple:

  * `AppleGlot <ftp://ftp.apple.com/developer/tool_chest/localization_tools/appleglot/appleglot_3.2_usersguide.pdf>`_
  * .plist - see `bug 633 <http://bugs.locamotion.org/show_bug.cgi?id=633>`_ and `plistlib <http://docs.python.org/library/plistlib.html>`_ for Python
* Adobe:

  * FrameMaker's Maker Interchange Format - `MIF <http://help.adobe.com/en_US/FrameMaker/8.0/mif_reference.pdf>`_ (See also `python-gendoc <http://lino.sourceforge.net/src/100.html>`_, and `Perl MIF module <http://search.cpan.org/~rst/FrameMaker-MifTree-0.075/lib/FrameMaker/MifTree.pm>`_)
  * FrameMaker's `Maker Markup Language <http://www.adobe.com/support/downloads/detail.jsp?ftpID=137>`_ (MML)
* Microsoft

  * Word, Excel, etc (probably through usage of OpenOffice.org)
  * `OOXML <https://en.wikipedia.org/wiki/OOXML>`_ (at least at the text level we don't have to deal with much of the mess inside OOXML).  See also: `Open XML SDK v1 <http://go.microsoft.com/fwlink/?LinkId=120908>`_
  * `Rich Text Format <https://en.wikipedia.org/wiki/Rich_Text_Format>`_ (RTF) see also
    `pyrtf-ng <http://code.google.com/p/pyrtf-ng/>`_
  * `Open XML Paper Specification <https://en.wikipedia.org/wiki/Open_XML_Paper_Specification>`_
  * .NET Resource files (.resx) - `Bug 396 <http://bugs.locamotion.org/show_bug.cgi?id=396>`_
* XML related

  * Generic XML
  * `DocBook <https://en.wikipedia.org/wiki/DocBook>`_ (can be handled by KDE's `xml2pot <http://linux.die.net/man/1/xml2pot>`_)
  * `SVG <http://www.w3.org/TR/SVG/>`_
  * `Android <https://en.wikipedia.org/wiki/Android_%28operating_system%29>`_ `resource files <http://code.google.com/android/devel/resources-i18n.html>`_ specifically `string resources <http://code.google.com/android/reference/available-resources.html#stringresources>`_ (`more background <http://www.linux-mag.com/id/7794>`_)
* `DITA <https://en.wikipedia.org/wiki/Darwin_Information_Typing_Architecture>`_
* `PDF <https://en.wikipedia.org/wiki/Portable_Document_Format>`_ see `spec <http://www.adobe.com/devnet/pdf/pdf_reference.html>`_, `PDFedit <http://pdfedit.petricek.net/en/index.html>`_
* `LaTeX <https://en.wikipedia.org/wiki/LaTeX>`_ - see `plasTeX <http://plastex.sourceforge.net/plastex/index.html>`_, a Python framework for processing LaTeX documents
* `unoconv <http://dag.wieers.com/home-made/unoconv/>`_ - Python bindings to OpenOffice.org UNO which could allow manipulation of all formats understood by OpenOffice.org.
* Trados:

  * TTX (`Reverse Engineered DTD <http://www.tracom.de/04/EN/techdoccenter/download/TRADOS_TTX-DTD.zip>`_, `other discussion <http://blogs.sun.com/timf/entry/beds_mattresses_and_open_standards>`_)
  * Multiterm XML `TSV to MiltiTerm conversion script <http://syntax.biz.pl/multiterm.html>`_ or `XLST <http://translationzone.eu/mtxml2txt.html>`_
* Tcl: .msg files.  `Good documentation <http://www.google.com/codesearch?hl=en&q=show:XvsRBDCljVk:M2kzUbm70Ts:D5EHICz0aaQ&sa=N&ct=rd&cs_p=http://www.scilab.org/download/4.0/scilab-4.0-src.tar.gz&cs_f=scilab-4.0/tcl/scipadsources/msg_files/AddingTranslations.txt>`_
* Installers:

  * NSIS installer: `Existing C++ implementation <http://trac.vidalia-project.net/browser/vidalia/trunk/src/tools>`_
  * WiX - MSI (Microsoft Installer) creator.  `Localization instructions <http://wix.mindcapers.com/wiki/Localization>`_, `more notes on localisation <http://www.mail-archive.com/wix-users@lists.sourceforge.net/msg15489.html>`_. This is a custom XML format, another one!
* catgets/`gencat <http://www.opengroup.org/onlinepubs/009695399/utilities/gencat.html>`_: precedes gettext, looking in man packages is the best information I could find.  Also `LSB requires it <http://dev.linuxfoundation.org/navigator/browse/cmd_single.php?cmd=list-by-name&Cname=gencat>`_. There is some info about the source (msgfile) format on `GNU website <http://www.gnu.org/software/libc/manual/html_node/The-message-catalog-files.html#The-message-catalog-files>`_
* Trados:

  * .tmw
  * .txt (You can interchange using TMX) `Format explanation <http://uk.dir.groups.yahoo.com/group/Tradosuser/message/2318?o=1&d=-1>`_ and `2 <http://translate.google.com/translate?js=y&prev=_t&hl=en&ie=UTF-8&layout=1&eotf=1&u=http%3A%2F%2Fwww.diemohrs.de%2Ftipps2_neu.html&sl=auto&tl=en>`_ with some `examples <http://slaci.komarom.net/roli/Trados/TRADOS%206.5.5.439%20Freelance%20+%20TRADOS%20MultiTerm%20iX%206.0.1.209/TRADOS%206.5.5.439%20Freelance/Program%20Files/TRADOS/T65_FL/Samples/TW4Win/>`_.
* :doc:`wml`
* `GlossML <http://www.maxprograms.com/glossml/glossml.pdf>`_
* Deja Vu External View: `Instructions sent to a translator <http://dvx.atril.com/docs/DVX/InstructionsExternalView.pdf>`_, `Description of external view options and process <http://simmer-lossner.com/lib/presentations/External_Proofreading_for_DVX.pdf>`_
* :doc:`Mozilla's l20n <l20n>`.

.. _pages/toolkit/formats#unlikely_to_be_supported:

Unlikely to be supported
========================

These formats are either: too difficult to implement, undocumented, can be processed using some intermediate format or used by too few people to justify the effort.  Or some combination or these issues.

.. Mentioned but we want them at the end of the TOC or to move them to developer docs

.. toctree::
   :maxdepth: 1
   :hidden:

   conformance
   base_classes
   quoting_and_escaping
