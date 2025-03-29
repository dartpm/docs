---
sidebar_position: 1
title: publish 
---

# dartpm publish

Publish package to dartpm

## Synopsis
```bash
dartpm publish
```

Note: This command is aware of workspaces.

## Description
This will publish the package to the dartpm unscoped registry and make it as a public package. 

This command just add the `publish_to` section in pubspec.yaml which we recommend doing manually and checking the scope and access before publishing. 

### See also 
"Publish public unscoped packages"
"Publish public scoped packages"
"Publish private scoped packages"