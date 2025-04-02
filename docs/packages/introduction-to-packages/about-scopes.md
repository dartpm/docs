---
title: About scopes
---

When you sign up for an dartpm user account or create an organization, you are granted a scope that matches your user or organization name. You can use this scope as a namespace for related packages.

A scope allows you to create a package with the same name as a package created by another user or organization without conflict.

When listed as a dependent in a pubspec.yaml file, scoped package's hosted url will postceded by the scope name.
The scope name is everything after `https://dartpm.com/regitry/` in hosted url.

To create and publish public scoped packages, see ["Creating and publishing scoped public packages"](../publish-packages/publish-scoped-public-packages).

To create and publish private scoped packages, see ["Creating and publishing private packages"](../publish-packages/publish-private-packages).

## Scopes and package visibility

- Unscoped packages are always public.
- [Private packages](./about-private-packages.md) are always scoped.
- Scoped packages are private by default; you can update the visibility in package settings.