# work-for-hire
Fork of ContractKiller template used by The OpenGov Foundation for contract work.  Frequently, we are contracting out work to others, so the terms here are inverted from the original.

This is a modified version of [Andy Clarke](http://stuffandnonsense.co.uk/)'s fantastic plain-English contract, the [ContractKiller (blog post)](http://stuffandnonsense.co.uk/projects/contract-killer/) [(source)](https://gist.github.com/malarkey/4031110).  We've had our lawyers run through it and clean up the language to be a bit more legal.

This document is being released with an open license, meaning it's **absolutely free to use**.  This will allow any person or organization - **for profit or not for profit** - to copy, edit, rewrite, and distribute it at no cost!  This is released under the original [CC-BY-SA license](./LICENSE).

## Disclaimer
This was created based on United States law, and if you're not in the US the policies here might not be legal wherever you are.

We are not lawyers, and cannot give you legal advice or tell you what is best for your organization.  You should have an actual lawyer review these documents before you use them in the first place.  If you have any questions, ask a lawyer.

We cannot be held responsible for any legal trouble that these documents get you into.  You're using them of your own accord.  We're providing them as-is with no warranty.  Seriously, please don't sue us.

## Available Files
We've provided this contract in a variety of formats to suit your needs:

* [Microsoft Word](https://rawgit.com/opengovfoundation/work-for-hire/master/docx/contract.docx)
* [PDF](https://rawgit.com/opengovfoundation/work-for-hire/master/pdf/contract.pdf)
* [HTML](https://rawgit.com/opengovfoundation/work-for-hire/master/html/contract.html)
* [Markdown](https://rawgit.com/opengovfoundation/work-for-hire/master/markdown/contract.md)

## Contributing

We welcome suggested edits to these documents!

We use Markdown as the primary format for these files, so you'll need to know a little before you begin. Don't worry - it's easy!  [Here's a quick guide.](https://guides.github.com/features/mastering-markdown/) If you've used a wiki, reddit, etc. it should be easy to pick up.  *Note that we _cannot_ accept changes directly made to other formats, only Markdown.*

If you don't want to learn Markdown and still want to contribute, feel free to [open an issue on this repo](./issues), or just [send us an email](mailto:sayhello@opengovfoundation.org).

### The Easy Way ###
You can edit the file directly using the link below, no account or GitHub experience needed!

*Coming Soon!*

### The Advanced Way ###
If you are familiar with GitHub, please fork the repo and send a pull request.

We use [pandoc](http://pandoc.org/) to generate the many formats we display.  If you don't have pandoc installed, that's ok!  Just send us a pull request with the updated markdown files.

If you have pandoc installed with pdfLaTeX, you can run the following command from the repository root to generate these files:

    for myfile in $( ls ./markdown ); do echo Converting $myfile; for fmt in html docx pdf; do filetrim=${myfile%???}; pandoc -o "./"$fmt"/"$filetrim"."$fmt -f markdown "./markdown/"$myfile; done ; done

