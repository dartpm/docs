---
title: About public packages
---

As an dartpm user or organization member, you can create and publish public packages that anyone can download and use in their own projects.

- Unscoped public packages exist in the global public registry namespace and can be referenced in a pubspec.yaml file with the publish_to: `https://dartpm.com`.
- Scoped public packages belong to a user or organization and must be preceded by the user or organization name when included as a dependency in a pubspec.yaml file:
  - publish_to: `https://dartpm.com/registry/username`
  - publish_to: `https://dartpm.com/registry/org-name`

Next steps

- "Creating and publishing scoped public packages"
- "Creating and publishing unscoped public packages"
- "Using npm packages in your projects"