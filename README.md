# RFC5246 in Markdown

This is a translation of RFC5246 into markdown, for use as a base document for TLS1.3 in the [TLS Working Group](http://datatracker.ietf.org/wg/tls/charter/).

## Requirements

You'll need:

* [kramdown-rfc2629](https://github.com/cabo/kramdown-rfc2629)
* [xmllint](http://xmlsoft.org/xmllint.html)
* [xml2rfc](http://xml.resource.org)
* [Saxon-B](http://sourceforge.net/projects/saxon/files/Saxon-B/)

## Use

Plain 'make' will process `draft.md` to produce both an HTML and a TXT-formatted Internet-Draft.

Do **not** edit the XML file; your changes will be lost.

When you publish a draft, run `make next` and a new XML file will be created.

## Notes

This is a reasonably close translation of the RFC into markdown. Changes in [the diff](draft-ietf-tls-tls13-00-from-rfc5246.diff.html) include:

* References to RFCs use the RFC number
* Definition lists are formatted differently; see [this 
  bug](https://github.com/cabo/kramdown-rfc2629/issues/3)
* There are a few references in blockquotes and similar places that haven't 
  been correctly converted
* Various formatting differences due to changes in RFC style over the years
* The references need checking for correct formatting.