---
sidebar_position: 2
title: Publish scoped public package
---

To share your code publicly in a user or organisation scope, you can publish public user-scoped or organisation-scoped packages/plugins to the dartpm registry. 

:::info[Note]
Before you can publish user-scoped dartpm packages, you must sign up for the dartpm account.
Additionally, to publish organisation-scoped package, you must create the dartpm user account, then create an npm organisation.
:::

## Creating and publishing scoped public packages

:::info[Note]
This article preassumes that you already have dartpm command line tool installed and login. To install, visit dartpm cli installation. To login, visit dartpm dartpm cli login.
:::

1. On the command line, create a flutter package.
    ```bash
    flutter create --template=package hello
    ```

2. Navigate to the root directory of your package: 
    ```bash
    cd hello    
    ```

3. Update `pubspec.yaml`
    ```yaml
    publish_to: "https://dartpm.com/registry/<scope-name>"
    access: "public" 
    ```
    - `scope-name` is <u>username</u> for user scoped and <u>org-name</u> for organisation scoped.
    - `access` is optional, 
        - if package is public set `access: "public"`,
        - if package is private set `access: "private"`, 
        - if `access` is missing the the package visibility will not be changed, if new package is published then the package will be private.


4. Run the publish command
    ```bash
    dart pub publish
    ```

:::tip[TIP]
When user is added to the new organisation, the user needs to run dartpm login again to set the new organisation. 
If you face any issue in publishing package, it is recommended to do dartpm login again.
:::

