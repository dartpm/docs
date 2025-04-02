---
sidebar_position: 1
title: About the developers team
---

The "developers" team is automatically created when you create an organisation. By default, the developers team has read/write access to all new packages created under the organisation's scope.

- Memvers added to the organisation, including the organisation owner, are automatically added to the developers team
- Any newly created packages under the organisation scope is publish in the developers team.

If an owner adds a new member to an organisation and does not want that member to be on the developers team, an owner can remove them.

:::info[Note]
Note: The developers team can no longer be removed from an organization for the following reasons:

It is the source of truth for all users, packages, and default permissions in an organization.
When you want to restrict write access, it is almost always better to set the default permissions to read-only and create separate teams for managing write permissions.
:::