---
sidebar_position: 3
title: Managing organization packages
---

As an organization member, you can manage packages within your organization's scope. This includes updating, deprecating, and transferring packages.

## Updating packages

To update a package:

1. Make your changes to the package code
2. Update the version in `pubspec.yaml`
3. Run `dart pub publish` to publish the new version

## Package visibility

You can change a package's visibility between public and private:

1. Navigate to the package page on dartpm
2. Click on "Settings"
3. Select "Make public"/"Make private" depending on the package status

:::info[Note]
Changing a package from public to private may affect users who are currently using the package. Make sure to communicate this change to your users.
::: 