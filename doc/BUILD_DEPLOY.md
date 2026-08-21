# Joshua-Hardware Build and Deployment

## Purpose and scope

Joshua-Hardware is currently a documentation-only placeholder. Its checked-in repository contains only `README.md` and `.gitignore`; there is no Makefile, source tree, package manifest, Docker/KAS/CMake/Rust/Python/Node configuration, deployment script, firmware, device tree, or automated test implementation to build.

The README explicitly records the missing board specification, Sitara/AM62x assets, STM32/companion-controller assets, device-tree sources, firmware, configuration manifest, install workflow, and validation fixtures. This guide documents that inventory without inventing commands.

## 1. Prerequisites

No repository-specific prerequisites are declared. A future implementation will need an agreed target board, toolchain, artifact ownership, and validation environment before setup can be prescribed.

## 2. Setup

There is no setup target or dependency manifest. From the leaf root, inspect the repository with ordinary source-control tools; do not expect a generated environment or build directory.

## 3. Build and compile

No Makefile or compiler configuration exists, so there is no supported build or compile command. `make` is not a documented workflow for this leaf.

## 4. Test and lint

No test or lint target exists and no automated tests are present. The README's inventory check is documentation only and is not a validation command for hardware.

## 5. Packaging and artifacts

No package, firmware, device-tree, binary, or other artifact is produced. There is no CPack, Docker image, SDK, or archive workflow.

## 6. Deployment, install, and run

No install, flash, deployment, or run command is defined. Do not flash or deploy neighboring HAL/OS artifacts as if they were produced by this repository. For current system-level work, consult Joshua-HAL for interface implementation and Joshua-OS for Yocto board/image integration.

## 7. Cleanup

There are no generated artifacts or repository-specific cleanup targets. Preserve the existing README and `.gitignore` when adding future implementation workflows.

## 8. Hardware, cloud, and manual verification caveats

This leaf cannot provide hardware or cloud verification because it contains no hardware assets or deployment contract. Before implementation is added, define board identity, device-tree/firmware ownership, toolchain, artifact format, flashing method, target credentials, and manual acceptance tests. Every current capability claim remains unimplemented or unknown as recorded in the existing README.
