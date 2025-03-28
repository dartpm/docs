---
sidebar_position: 5
title: Semantic versioning
---

To keep the dart ecosystem healthy, reliable, and secure, every time you make significant updates to the dart package you own, we recommend publishing a new version of the package with an updated version number in the pubspec.yaml file the follows the semantic versioning spec. Following the semantic versioning spec helps other developers who depend on your code understnad the extent of changes in a given version, and adjust their own code ig necessary.

:::info[Note]
If you introduce a change that breaks a package dependency, we strongly recommend incrementing the version major number; see below for details.
:::

Code status | Stage | Rule | Example version |
--- | --- | --- | --- |
First release | New product | Start with 1.0.0 | 1.0.0
Backward compatible bug fixes | Patch release | Increment the third digit | 1.0.1
Backward compatible new features | Minor release | Increment the middle digit and reset last digit to zero | 1.1.0
Changes that break backward compatibility | Major release | Increment the first digit and reset middle and last digits to zero | 2.0.0

## Using semantic versioning to specify update types your package can accept
You can specify which update types your package can accept from dependencies in your package's pubspec.yaml file.

For example, to specify acceptable version ranges up to 1.0.4, use the following syntax:

Patch releases: 1.0 or 1.0.x or ~1.0.4
Minor releases: 1 or 1.x or ^1.0.4
Major releases: * or x
