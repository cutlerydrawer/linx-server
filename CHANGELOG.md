# Changelog

## 3.1.0 - 2025-06-02

### Other changes

* Dependency updates

## 3.0.0 - 2022-02-01

### Breaking changes

* **Breaking:** Remove support for S3 backends.
* **Breaking:** `PUT` uploads that don't request a JSON response will now return the raw URL.

### Other changes

* Update Blackfriday to v2.
* API keys can now be passed as bearer tokens, to aid interoperability with other standards-compliant software.

## 2.3.9 - 2021-09-02

### Other changes

* Static files and templates are now embedded in the linx-server binary.
  This means they can't be customised at run-time, but makes it much
  easier to deploy (just a single binary).
* Update to Go 1.17.
* Various minor updates to dependencies.

