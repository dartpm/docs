---
title: About private packages
---

With dartpm private packages, you can use the dartpm registry to host code that is only visible to you and chosen collaborators (for user private package, the collaborator is comming soon), allowing you to manage and use private code alongside public code in your projects.

Private packages always have a scope, and scoped packages are private by default.

- User-scoped private packages can only be accessed by only you using registry "https://dartpm.com/registry/username"

- Organization-scoped private packages can only be accessed by teams that have been granted read or read/write access. Registry for the organiation is "https://dartpm.com/registry/org-name"
    
For more information, see "Managing team access to organization packages".

## Next steps
- ["Creating and publishing private packages"](../publish-packages/publish-private-packages)
- ["Using npm packages in your projects"](../getting-packages/downloading-and-installing-packages-locally)