---
sidebar_position: 1
title: Publish unscoped public package
---

As a dartpm user, you can create unscoped packages to use in your own projects and publish them to the dartpm public registry for others to use in their. Unscoped packages are always public and are refferd to by the package name only.

## Creating and publishing an unscoped public package

:::info[Note]
This article preassumes that you already have dartpm command line tool installed and login. To install and setup, visit ["dartpm cli installation"](../../dartpm-cli/install-and-setup.md)
:::

1. On the command line, create a directory for your package.
    ```bash
    flutter create --template=package hello
    ```

2. Navigate to the root directory of your package: 
    ```bash
    cd hello    
    ```

3. Update `pubspec.yaml`
    ```yaml
    publish_to: "https://dartpm.com"
    ```

4. Run the publish command
    ```bash
    dart pub publish
    ```
