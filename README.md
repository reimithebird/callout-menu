# Callout menu

> [!NOTE]
> **This is a fixed fork.** The [original plugin](https://github.com/anareaty/callout-menu) broke in Obsidian 1.13 due to a CodeMirror upgrade: the callout block widget moved from `el.cmView` to `el.cmTile`, so right-clicking a callout threw `TypeError: Cannot read properties of undefined (reading widget)` and the context menu never opened. This fork patches all widget accesses to use `el.cmTile?.widget ?? el.cmView?.widget`, restoring compatibility with Obsidian 1.13+ while keeping support for older versions. The fix was also submitted upstream as [PR #14](https://github.com/anareaty/callout-menu/pull/14) — if it gets merged and released, this fork can be retired.

This plugin can be useful for people who use a lot of custom callouts instead of default ones and want to have ability to quickly change callout types from context menu. Now you can chose which callout types will be shown in the menu. Also it adds the ability to easily add or remove callout metadata and "+" or "-" signs for collapsing. 

![](screenshots/Callout-menu.png)

## How to use

Open plugin settings an enter the list of callout types and metadata types you want to appear in the context menu.

## Installation via BRAT
1. Install the BRAT plugin from "Community plugins" page.
2. Go to the BRAT settings.
3. Click "Add Beta Plugin" button.
4. Paste the following URL in the text field: https://github.com/anareaty/callout-menu.
5. Make sure that "Enable after installing the plugin" is checked.
6. Click "Add Plugin" button.
