---
sidebar_position: 1
title: Install and setup cli
---

## Description

To publish and install packages to and from the public dartpm registry, 
you must install dart command line interface using https://dart.dev/get-dart.

## Checking your version of dartpm

To see if you already have dartpm installed and check the installed version, run the following commands:

```bash
dartpm
```

## Install using dart command line tool
```bash
dart pub global activate --source hosted --hosted-url "https://dartpm.com" dartpm
```

## Setup session

To read and write packages to your account, you need to first setup the dartpm cli tool. 
```bash
dartpm login
```

dartpm do not store any secret token other then inside dart token manager. This imporves risk of loosing secrets. 

:::info[Note]
If you are added to new organisation or removed from the organisation, do `dartpm login` again to sync the sessions. 
:::


