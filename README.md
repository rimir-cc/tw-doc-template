# Doc Template

> Branded documentation system for rimir plugins

Renders plugin documentation with a consistent layout featuring a dark header, tab navigation, breadcrumbs, and an auto-discovery hub that lists all documented plugins.

## Key features

* **Auto-discovery hub** -- card grid grouped by category, finds all documented plugins automatically
* **Branded page layout** -- header, breadcrumb, tabs, and footer for consistent presentation
* **Field-based discovery** -- no tags needed, uses `rdt.*` fields for metadata
* **Callout boxes** -- four types: info, warning, tip, danger
* **In-place navigation** -- seamless browsing when accessed from the hub
* **Related plugins footer** -- links to related plugins at the bottom of each page

## Prerequisites

* theme plugin (for CSS classes)

## Quick start

Create `doc-overview.tid` in your plugin with `rdt.plugin-key`, `rdt.section`, `rdt.plugin-name`, `rdt.plugin-subtitle`, `rdt.hub-category` fields. The version is read automatically from `plugin.info`. Transclude `$:/plugins/rimir/doc-template/templates/page` and fill the `body` slot. The hub auto-discovers it.

## License

MIT -- see [LICENSE.md](LICENSE.md)
