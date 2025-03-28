---
sidebar_position: 3
title: Publish private package
---

To share your code with a limited set of users or teams, you can publish private user-scoped or organisaition-scoped packages to the dartpm registry.

For more information on scopes and private package, see "About scopes" and "About private packages".

:::info[Note]
Before you can publish private user-scoped dartpm packages, you must sign up for the dartpm account.
Additionally, to publish organisation-scoped package, you must create the dartpm user account, then create an npm organisation.
:::

## Creating and publishing private packages

:::info[Note]
This article preassumes that you already have dartpm command line tool installed and login. To install, visit dartpm cli installation. To login, visit dartpm dartpm cli login.
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
    publish_to: "https://dartpm.com/registry/<scope-name>"
    ```
    - `scope-name` is <u>username</u> for user scoped and <u>org-name</u> for organisation scoped.
    - `scope-name` is <u>username</u> for user scoped and <u>org-name</u> for organisation scoped.

4. Run the publish command
    ```bash
    dart pub publish
    ```

:::tip[TIP]
When user is added to the new organisation, the user needs to run dartpm login again to set the new organisation. 
If you face any issue in publishing package, it is recommended to do dartpm login again.
:::

