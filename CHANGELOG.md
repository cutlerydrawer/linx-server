# Changelog

## 3.4.1 - 2026-03-31

### Bug fixes

* Fix `redirect` and `randomize` query parameters not working when passed as flag-style (no value).

## 3.4.0 - 2026-03-31

### Other changes

* Accept API key query parameter in both `Linx-Api-Key` and `linx-api-key` forms.

## 3.3.0 - 2026-03-31

### Other changes

* Allow POST uploads with a raw file body (in addition to multipart and URL-encoded forms).
* Add `redirect` query parameter to return a `201 Created` with a `Location` header on upload.
* Replace custom CSRF checks with Go 1.25's `http.CrossOriginProtection` (`Sec-Fetch-Site` based).
* Update hotlink protection to use `Sec-Fetch-Site` instead of `Referer` header.

## 3.2.0 - 2026-03-31

### Other changes

* Add `-getapikey` option to allow passing the API key via the `Linx-Api-Key` query parameter.
* Dependency updates.

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

