# vNext

# v3.0.0

* **Breaking:** Remove support for S3 backends.
* Update Blackfriday to v2.
* API keys can now be passed as bearer tokens, to aid interoperability with other standards-compliant software.
* **Breaking:** `PUT` uploads that don't request a JSON response will now return the raw URL.

# v2.3.9

* Static files and templates are now embedded in the linx-server binary.
  This means they can't be customised at run-time, but makes it much
  easier to deploy (just a single binary).
* Update to Go 1.17.
* Various minor updates to dependencies.

