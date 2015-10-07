CONTRIBUTING
============

There are several ways you can help contribute to meza.

## Report bugs

You may help us by reporting bugs and feature request via the issue tracker. Please remember to always provide information about your environment and any error messages you receive.

## Improve documentation

meza is in very early stages of development, and as such the documentation may become quickly out-of-date. If you see any issues with documentation please submit an issue and/or an update to the documentation.

## Provide patches

We have a long list of features to add and bugs to fix. We'd greatly appreciate any assistance making meza better.

## Test development builds

At any given time there are several new builds being considered for approval in our Pull Requests section. Please consider attempting to build these. The authors consider them ready for test if they are marked by the green "please review" label. If there are no pull requests marked "please review" we're always looking for more eyes on our master branch.

### Testing requirements

#### Minimal requirements

These tests should be performed on all changes

* Create page with wikitext editor
* Create page with VisualEditor
* Verify adding images to pages with VisualEditor
* Verify adding edit summary in VisualEditor
* Verify search works
* Verify ElasticSearch works by searching with a typo (e.g. search for "Test Paeg" when looking for "Test Page")
* Verify file uploads work
* Verify thumbnailing works (upload a larger image and verify small images are generated)

#### Desired testing

The following tests should be performed if time allows, or if a change is likely to affect any test.

* Verify PDFHandler functioning (PDF images shown on PDF file pages)
* Verify image security: users unable to view images when not logged in


#### Pre-release testing requirements

These tests should be performed prior to each release of meza, or any time  change is likely to affect any test.

* Repeat all tests for CentOS 6 32-bit
* Repeat all tests for CentOS 6 64-bit
* Repeat all tests for CentOS 7 (64-bit only)
* Create semantic properties in several pages, perform #ask query and verify results