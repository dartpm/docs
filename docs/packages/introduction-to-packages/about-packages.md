---
title: About dart and flutter packages
---

# About Dart and Flutter Packages

In the world of Dart and Flutter development, packages are essential building blocks that allow developers to share, reuse, and manage code efficiently. Understanding the distinction between packages and modules is important for effectively using dartpm to manage your Dart and Flutter packages in a private registry.

## About Packages
A package in the Dart ecosystem is a collection of Dart code, libraries, tools, or assets bundled together. For a package to be published and used, it must include a pubspec.yaml file, which contains essential metadata such as the package name, version, dependencies, and other configuration details.

Packages can be unscoped or scoped to a user or organization, and scoped packages can be private or public. For more information, see
- ["About scopes"](#)
- ["About private packages"](#)
- ["About public packages"](#)

## Package Formats
A Dart or Flutter package published on dartpm is typically structured as a folder containing a Dart project or library, described by a pubspec.yaml file.

## Dart vs. Flutter Packages
Dart packages are core libraries or tools built using Dart. They might be used in both server-side Dart applications and in Flutter applications.
Flutter packages are specialized packages designed specifically for Flutter apps, often containing UI components, widgets, or Flutter-specific plugins. These packages can also include Dart code but are optimized to work within the Flutter framework for mobile, desktop, or web applications.
While dartpm allows both Dart and Flutter packages to be managed securely, you can expect a higher level of integration for Flutter packages, as they often require additional resources such as platform-specific code or assets.

## Using Packages in dartpm
Once you’ve published your Dart or Flutter packages on dartpm, you can share them with your team, colleagues, or within your organization. These packages can be installed and used by importing them into your Dart or Flutter projects using the pub get command or adding them directly to your pubspec.yaml file.

By leveraging dartpm, you maintain full control over the distribution and access of your packages. You can ensure that your private code remains secure while facilitating collaboration among your development teams.