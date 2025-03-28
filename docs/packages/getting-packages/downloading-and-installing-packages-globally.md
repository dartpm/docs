---
sidebar_position: 2
title: Downloading and installing packages globally
---

You can install a package gloabally if you want to depend on the package from your own packages.

:::info[Note]
dartpm cli is using dart cli tool, so the dartpm add is running complex dart command. 
dart command can only be used if dartpm cli is logged in or granular token is set for the scope. 
:::

## Installing an unscoped package
Unscoped packages are always public, which means they can be downloaded and installed by anyone. To install a public package, on the command line, run

```bash
dartpm add -g package-name
OR
dart pub global activate --source hosted --hosted-url "https://dartpm.com" <package-name>
```

## Installing a scoped public package
Scoped public packages can be downloaded and installed by anyone, as long as the scope name is refenced during installation:

```bash
dartpm add -g scope/package-name
OR
dart pub global activate --source hosted --hosted-url "https://dartpm.com" <package-name>
```

## Installing a scoped private package
Scoped private packages can be downloaded and installed by only who have access. 

### Installing package using dartpm account
User can install the package which user have access to.

```bash
dartpm add -g scope/package-name
OR
dart pub global activate --source hosted --hosted-url "https://dartpm.com/registry/<scope>" <package-name>
```


### Installing package using granular token
Orgnisation admin can create the granular token to give fine tune access to selected package with READ or WRITE access. 

1. Set the granular token for the scope.
```bash
dart pub token add https://dartpm.com/registry/<scope>
Enter secret token: <Type token on stdin>
 Requests to "https://dartpm.com/registry/<scope>" will now be 
 authenticated using the secret token.
```

2. Install the package.
```bash
dartpm add -g <scope>/<package-name>
OR
dart pub global activate --source hosted --hosted-url "https://dartpm.com/registry/<scope>" <package-name>
```