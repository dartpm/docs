---
sidebar_position: 2
title: Publish scoped public package
---

To share your code publicly in a user or organization scope, you can publish public user-scoped or organization-scoped packages/plugins to the dartpm registry. 

:::info[Note]
Before you can publish user-scoped dartpm packages, you must sign up for the dartpm account.
Additionally, to publish organization-scoped package, you must create the dartpm user account, then create an npm organization.
:::

## Creating and publishing scoped public packages

:::info[Note]
This article preassumes that you already have dartpm command line tool installed and login. To install and setup, visit ["dartpm cli installation"](../../dartpm-cli/install-and-setup.md)
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
    ```
    - `scope-name` is <u>username</u> for user scope and <u>org-name</u> for organization scope.


4. Run the publish command
    ```bash
    dart pub publish
    ```

5. If organization don't allow private packages then the published package will be public, otherwise all the published package are private and there status can be changed from package settings in web.

:::tip[TIP]
When user is added to the new organization, the user needs to run dartpm login again to set the new organization. 
If you face any issue in publishing package, it is recommended to do dartpm login again.
:::

