Citation Backlinks Filter
==================================================================

[![GitHub build status][CI badge]][CI workflow]

This filter modifies the bibliography, adding backlinks to the
locations in the text where an item is cited.

[Lua filters]: https://pandoc.org/lua-filters.html
[CI badge]: https://img.shields.io/github/workflow/status/tarleb/citation-backlinks/CI?logo=github
[CI workflow]: https://github.com/tarleb/citation-backlinks/actions/workflows/ci.yaml

Usage
------------------------------------------------------------------

This filter should be invoked after `citeproc`, e.g.

    pandoc --citeproc --lua-filter citation-backlinks.lua ...

Users of Quarto can install this filter as an extension with

    quarto install extension tarleb/citation-backlinks

and use it by adding `citation-backlinks` to the `filters` entry
in their YAML header.

```` yaml
---
filters:
  - citation-backlinks
---
````


License
------------------------------------------------------------------

This pandoc Lua filter is published under the MIT license, see
file `LICENSE` for details.
