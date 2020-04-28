# Pangeo Gallery Template

This repository stores an example gallery repo for the Pangeo Gallery.
It is configured to automatically build itself using
[binderbot](https://github.com/pangeo-gallery/binderbot).
It is linked, via a git submodule, the the
[gallery website repo](https://github.com/pangeo-gallery/pangeo-gallery).
Whenever the notebooks are updated in this, repository
dispatch is used to trigger a gallery rebuild. This keeps
[gallery.pangeo.io](http://gallery.pangeo.io) always in sync with this repo.

The repo contains the following elements:

- A set of jupyter notebooks, numbered in the order that we want them to
  appear on the gallery website.
- A configuration file, `binder-gallery.yaml`, which provides important
  configuration parameters (see [pangeo gallery documentation](http://gallery.pangeo.io)).
- A thumbnail image (`thumbnail.png`), a 200 x 200 px image which represents
  the gallery content.
- Github workflows, which make the magic happen! (Don't touch these.)
