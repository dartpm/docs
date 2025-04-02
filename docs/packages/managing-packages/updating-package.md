---
sidebar_position: 3
title: Updating package
---

When you make significant changes to a published package, we recommend updating the version number to communicate the extent of changes to other who rely on your code.

1. Update the version number in pubspec.yaml
```
version: 1.0.X
```

2. Publish the new version
```bash
dartpm publish
```
