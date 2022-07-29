# Upgrading to Project Factory v14.0

The v14.0 release of Project Factory is a backwards compatible release.

### New `random_project_id_string_method` in addition to `random_project_id`

A new `random_project_id_string_method` alternative to `random_project_id`.  It
includes a larger collusion domain for use with CI.  It defaults to 4
characters, but the length can be adjusted with `random_project_id_length`.  If
both `random_project_id` and `random_project_id_string_method` are enabled, the
new `random_project_id_string_method` will be used.
