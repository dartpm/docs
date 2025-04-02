---
sidebar_position: 1
title: Creating and publishing an organization scoped package
---

As an organisation member, you can create and publish public and private packages within the organisation's scope. 

:::info[Note]
TODO: User id already loggedin
:::

## Creating an organisation scoped package.

1. On the command line, create a flutter package.
    ```bash
    flutter create --template=package hello
    ```

2. Navigate to the root directory of your package: 
    ```bash
    cd hello    
    ```

3. To create an organisation scoped package, update `pubspec.yaml`.
    ```yaml
    publish_to: "https://dartpm.com/registry/<scope-name>"
    ```

## Publishing a private organisation scoped package
By default, `dart pub publish` will publish a scoped package as private.

Be default, any scoped package is published as private. However, if you have an organisation that does not have the Private Packages feature, `dart pub publish` will fail unless you pass the access flag.

1. On the command line, navigate to the package directory. 

2. Run `dartpm publish`.

Private packages will say `private` below the package name on the npm website.

## Publishing a publish organisation scoped package

To publish an organization scoped package as public, use `dartpm publish --access public`.

On the command line, navigate to the package directory.

Run `dartpm publish --access public`.

Public packages will say public below the package name on the npm website.

