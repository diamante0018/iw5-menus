# IW5 Menus: A collection of Quake III: Arena style menus

The menus available in this repository are "stock" menus created for Modern Warfare 3 (2011) and were extracted using [OAT][oat-link].

One of the primary challenges in utilizing these extracted menus is their near-impossibility of being reutilized by the tool itself. This difficulty arises from several mistakes made by the original developers of the menus. It's unclear whether these mistakes were made during their development or if the tool they used to link the fast files was flawed. However, various "unexpanded" macros can be observed throughout the menus, along with numerous other errors.

This repository comprises menus that have undergone manual correction and no longer contain these errors. Consequently, it should be feasible to relink the fast files using OAT without any adjustments to the assets found within this repository.

## How to use OAT

You should invoke the linker with the following options:

| Argument                    | Description                                    |
|:----------------------------|:-----------------------------------------------|
| `--load=PATH`               | Required. Loads the original fast file into memory. It is needed to find material and images not included in this repository. |
| `--menu-permissive`         | Required. Allows the tool to permit some "weird" syntax. |
| `--menu-no-optimization`    | Optional.                                      |

[oat-link]:     https://github.com/Laupetin/openassettools
