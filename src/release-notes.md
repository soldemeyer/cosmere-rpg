### Release 2.1.2 🔧
<sup>24th June 2026</sup>

Compatibility update for Foundry VTT v14. No new features — this release updates the system to run correctly on Foundry v14 and fixes a crash that occurred when rolling damage.

#### 🛠️ Full Changelog

##### 🐛 Bug Fixes

* Updated system compatibility for Foundry VTT v14
* Fixed a crash ("Cannot assign to read only property 'effects'") that occurred when rolling damage in Foundry v14
* Fixed a deprecation warning for `KeyboardManager` now namespaced under `foundry.helpers.interaction.KeyboardManager` in Foundry v14
* Updated `TextEditor.enrichHTML` and `TextEditor.getDragEventData` calls to use the new v14 namespaced API
* Removed deprecated `CONFIG.ActiveEffect.legacyTransferral` setting removed in v14
* Updated sheet registration to use the new v14 `foundry.documents.collections` API

— **Team Metalworks**

---

### Release 2.1.0 ✨
<sup>15th May 2026</sup>

Minor release which includes a few new features and some non-breaking changes to existing ones. Most notably we have added some very limited resizing ability to player character sheets and the ability to collapse various sections of the list tabs (such as actions and equipment). Yep, at long last, some of you with smaller screens can see your whole sheet. Further work on enhancing sheets to allow more dynamic font sizes and scalings is in the works, but still a bit away. Hopefully this helps people in the meantime!

#### 🛠️ Full Changelog

##### 📝 Features

* Token Configuration defaults are now set by system ([#278](https://github.com/the-metalworks/cosmere-rpg/issues/278))
* Actor action and equipment tab sections can now collapse for easier sheet navigation ([#541](https://github.com/the-metalworks/cosmere-rpg/issues/541) & ([#715](https://github.com/the-metalworks/cosmere-rpg/issues/715)))
* Encumbrance is now tracked on the character sheet (([#648](https://github.com/the-metalworks/cosmere-rpg/issues/648)))
* Events can now be toggled on/off to better control their activation ([#661](https://github.com/the-metalworks/cosmere-rpg/issues/661))
* The actor sheet for player characters can now be resized within certain bounds ([#636](https://github.com/the-metalworks/cosmere-rpg/issues/636))

##### 🐛 Bug Fixes

* Derived values no longer become NaN upon stats exceeding 10 using active effects ([#684](https://github.com/the-metalworks/cosmere-rpg/issues/684))
* Weapon range fields now appear as expected when selecting attack type ([#705](https://github.com/the-metalworks/cosmere-rpg/issues/705))
* Grant Items handler on event rules can now scroll when necessary ([#713](https://github.com/the-metalworks/cosmere-rpg/issues/713))

— **Team Metalworks**
