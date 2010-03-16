= HISPID 5 README =

HISPID 5, documented more fully at http://hiscom.chah.org.au/wiki/HISPID_5
represents a major change to the way Australian herbaria will transfer data. It
is an XML Schema based on the ABCD Schema developed by TDWG, the global
biodiversity informatics standards group, http://www.tdwg.org/activities/abcd.

== Schema ==

The HISPID 5 schema is a copy of ABCD 2.06b that has been altered to allow
overriding of elements to conform to HISPID vocabularies. It imports the
HISPID5extension.xsd document for the custom elements and types that are
referenced in the relevant extension slots in ABCD. The extension schema itself
references ABCD 2.06b in order to be able to override some types.

== Examples ==

There are a number of example XML instance documents that contain the same
example data as originally supplied in the HISPID 3 documentation at:
http://plantnet.rbgsyd.nsw.gov.au/HISCOM/HISPID/HISPID3/H3.html#_Toc366998610.

exampleABCD.xml is a vanilla ABCD document. exampleHISPID5standard.xml is the
same document as above (i.e. without any HISPID 5 extensions in use), except
that the schemaLocation and other document attributes are for HISPID 5. This
proves that HISPID 5 is a true ABCD document when no HISPID 5 elements are used.
exampleHISPID5extended.xml is the HISPID 3 data implemented as HISPID 5 with
HISPID 5 extensions used in place of their ABCD counterparts.

== Notes ==

The latest schema can always be downloaded from the subversion repository at
http://big.sourceforge.net.

Errors in Eclipse's XML Schema editor like "cvc-elt.1: Cannot find the
declaration of element 'DataSets'" can be addressed by following the
instructions at
http://dev.eclipse.org/newslists/news.eclipse.webtools/msg05916.html.
Additionally, deleting cached copies and trying again resolves the problem.