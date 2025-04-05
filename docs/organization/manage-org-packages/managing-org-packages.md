---
sidebar_position: 3
title: Managing organization packages
---

As an organization member, you can manage packages within your organization's scope. This includes updating, deprecating, and transferring packages.

## Updating packages

To update a package:

1. Make your changes to the package code
2. Update the version in `pubspec.yaml`
3. Run `dartpm publish` to publish the new version

## Deprecating packages

To deprecate a package:

1. Navigate to the package page on dartpm
2. Click on "Settings"
3. Select "Deprecate package"
4. Choose whether to deprecate all versions or specific versions
5. Add a deprecation message explaining why the package is being deprecated

## Transferring packages

To transfer a package to another organization:

1. Navigate to the package page on dartpm
2. Click on "Settings"
3. Select "Transfer package"
4. Enter the name of the target organization
5. Confirm the transfer

:::warning[Note]
Only organization owners can transfer packages. The target organization must have the appropriate permissions to receive the package.
:::

## Package visibility

You can change a package's visibility between public and private:

1. Navigate to the package page on dartpm
2. Click on "Settings"
3. Select "Change visibility"
4. Choose the new visibility setting
5. Confirm the change

:::info[Note]
Changing a package from public to private may affect users who are currently using the package. Make sure to communicate this change to your users.
::: 