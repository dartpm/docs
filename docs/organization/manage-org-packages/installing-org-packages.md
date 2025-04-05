---
sidebar_position: 2
title: Installing organization packages
---

To install a package from your organization, you need to authenticate with dartpm and have the appropriate permissions.

## Installing private packages

To install a private package from your organization:

1. Make sure you are logged in to dartpm:
    ```bash
    dartpm login
    ```

2. Install the package using the package name:
    ```bash
    dartpm add <scope>/<package-name>
    ```

## Installing public packages

Public packages from your organization can be installed without authentication:

```bash
dartpm add <scope>/<package-name>
```

## Troubleshooting

If you encounter issues installing packages:

1. Verify you are logged in to dartpm, use `dartpm doctor`
2. Check that you have the correct permissions in your organization
3. Ensure the package name and version are correct
4. Check your internet connection
5. Try `dartpm login` again

For more help, contact your organization administrator or dartpm support. 