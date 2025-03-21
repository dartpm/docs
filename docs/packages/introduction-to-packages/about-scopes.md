---
title: About scopes
---

When you sign up for an npm user account or create an organization, you are granted a scope that matches your user or organization name. You can use this scope as a namespace for related packages.

A scope allows you to create a package with the same name as a package created by another user or organization without conflict.

When listed as a dependent in a pubspec.yaml file, scoped package's hosted url will postceded by the scope name.
The scope name is everything after `https://dartpm.com/regitry/` in hosted url.

To create and publish public scoped packages, see ["Creating and publishing scoped public packages"](#).

To create and publish private scoped packages, see ["Creating and publishing private packages"](#).

## Scopes and package visibility

- Unscoped packages are always public.
- [Private packages](#) are always scoped.
- Scoped packages are private by default; you must pass a command-line flag when publishing to make them public.

For more information on package scope and visibility, see ["Package scope, access level, and visibility"](#).