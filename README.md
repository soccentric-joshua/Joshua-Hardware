# Joshua-Hardware

## Project Summary

Joshua-Hardware is the hardware-definition leaf of the Joshua project tree. The repository currently
contains only this README, so it does not yet expose drivers, board-support source, device-tree
files, firmware, schematics, configuration manifests, build scripts, or automated tests that can be
inspected here. That absence is itself important for consumers of the wider Joshua stack: Joshua-HAL
and Joshua-OS document target hardware assumptions, but this repository does not currently provide
an implementation boundary for those assumptions.

The intended role can be inferred from the neighboring project structure: a hardware leaf would
normally hold board-specific assets or a canonical record of the Joshua Sitara/STM32 target, while
the HAL would consume device paths and the OS would package the board through Yocto. No such
contract is present in the checked-in files, so this README records the repository as an inventory
placeholder rather than inventing capabilities. There is no setup command to run and no test command
to cite beyond checking that the repository remains empty of implementation files. Before this leaf
can be treated as a delivered component, the project needs an agreed scope, target boards, ownership
of device-tree and firmware assets, a build/install path, and tests or validation fixtures. Until
then, users should consult Joshua-HAL for hardware interface abstractions and Joshua-OS for
image/build integration, while treating any hardware claims in sibling documentation as external
dependencies rather than features implemented here. Every row below leaves physical verification
open.

## Feature Inventory

| # | Name / Description | Implemented? | Test Coverage? | Manual Test |
| --- | --- | --- | --- | --- |
|   1 | Repository README and project placeholder                | Implemented                        | Not applicable  | [ ] Manual verification required |
|   2 | Joshua board hardware specification                      | Planned                            | None identified | [ ] Manual verification required |
|   3 | Sitara/AM62x board support assets                        | Unknown                            | None identified | [ ] Manual verification required |
|   4 | STM32 or companion-controller assets                     | Unknown                            | None identified | [ ] Manual verification required |
|   5 | Device-tree sources or overlays                          | Not implemented in this repository | None identified | [ ] Manual verification required |
|   6 | Firmware or binary hardware blobs                        | Not implemented in this repository | None identified | [ ] Manual verification required |
|   7 | Hardware configuration manifest                          | Not implemented in this repository | None identified | [ ] Manual verification required |
|   8 | Build/install workflow                                   | Not implemented in this repository | None identified | [ ] Manual verification required |
|   9 | Hardware validation fixtures                             | Not implemented in this repository | None identified | [ ] Manual verification required |
|  10 | User and contributor documentation beyond this inventory | Planned                            | None identified | [ ] Manual verification required |

## Current Limitation

The repository is documentation-only at scan time. No build or test command can be honestly
prescribed until implementation files and project ownership are added.
