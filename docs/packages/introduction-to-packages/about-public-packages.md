---
title: About public packages
---

As an dartpm user or organisation user(Member/Admin), you can create and publish public packages that anyone can download and use in their own projects.

- Unscoped public packages exist in the global public registry namespace and can be referenced in a pubspec.yaml file using:
  ```
  publish_to: "https://dartpm.com"
  ```
- Scoped public packages belong to a user or organisation and must be preceded by the user or organisation name when included as a dependency in a pubspec.yaml file:
  - For user account
    ```
    publish_to: "https://dartpm.com/registry/username"
    access: "public"
    ```
  - For organisation
    ```  
    publish_to: "https://dartpm.com/registry/org-name"
    access: "public"
    ```
  
:::info[Note]
Is the package is unscoped, the package is public and `access` field is ignored, otherwise for scoped packages, access can be used to define if package is 'public' or 'private'. By default access is 'private'
:::


Next steps

- "Creating and publishing scoped public packages"
- "Creating and publishing unscoped public packages"
- "Using npm packages in your projects"