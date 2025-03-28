---
title: About private packages
---

With dartpm private packages, you can use the dartpm registry to host code that is only visible to you and chosen collaborators (for user private package, the collaborator is comming soon), allowing you to manage and use private code alongside public code in your projects.

Private packages always have a scope, and scoped packages are private by default.

- User-scoped private packages can only be accessed by you.
    ```
    publish_to: "https://dartpm.com/registry/username"
    ```

- Organisation-scoped private packages can only be accessed by teams that have been granted read or read/write access. For more information, see "Managing team access to organisation packages".
    ```  
    publish_to: "https://dartpm.com/registry/org-name"
    ```

## Next steps
- "Creating and publishing private packages"
- "Using npm packages in your projects"