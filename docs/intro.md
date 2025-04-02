---
sidebar_position: 1
---

# About dartpm

dartpm is a Dart and Flutter package management platform designed for developers to easily share, store, and manage packages in a secure environment. Whether you're working on personal projects or collaborating with teams in organizations, dartpm offers a reliable and efficient way to manage your Dart and Flutter packages.

dartpm consists of three main components:

- **The Website**  
  The web interface allows users to manage their Dart and Flutter packages, set up profiles, and organize teams. You can also use the website to create or manage organizations, invite members, and manage permissions for both public and private packages.

- **The Command Line Interface (CLI)**  
  The CLI is the important tool for interacting with dartpm. It allows users to publish and retrieve Dart and Flutter packages, manage authentication, and interact with dartpm from the terminal. You can also use the CLI to automate package management tasks.

- **The Registry**  
  The dartpm registry is a secure, private repository for hosting and managing Dart and Flutter packages. The registry supports both public and private packages, with access controls in place to ensure that only authorized users can access certain packages.

## Use dartpm to...

- Publish and share Dart and Flutter packages with other developers and organizations.
- Store and manage your Dart and Flutter packages securely in a private registry.
- Collaborate with your team by creating organizations and sharing packages privately.
- Restrict access to specific developers or teams with organization-based access controls.
- Maintain multiple versions of your Dart and Flutter packages and manage dependencies.
- Set up automated workflows using dartpm's CLI for package management tasks.
- Ensure the security of your code by utilizing the robust security measures of the dartpm server.

## Getting Started

To get started with dartpm, you can create an account using SSO. Once your account is set up, you can begin using the command line tool to publish and manage your Dart and Flutter packages.

To get started with dartpm, follow these steps:

1. [Create an account](https://dartpm.com/login) using SSO.
2. [Install](./dartpm-cli/install-and-setup.md) the dartpm CLI on your machine.
3. Begin managing your Dart and Flutter packages and collaborating with your team.

## Sharing Packages and Collaborating with Others

dartpm allows you to publish both public and private Dart and Flutter packages. While you can share public packages with anyone, only paid users can publish and manage private packages.

You can organize your projects into teams by creating organizations. Each organization can have different permissions for package access, allowing you to control who can publish, edit, or access your private packages. Organizations can also share packages with other companies via secure tokens.

If you're working within a company, dartpm enables you to share packages with other organizations by creating a fine tuned granular token.

## Security and Privacy

dartpm is committed to providing a secure environment for your Dart and Flutter packages. Our servers are designed with the latest security measures to ensure that only authorized users can access your packages.

- We do not collect any personal information during account creation or usage.
- Packages stored on dartpm are protected by strict access controls.
- Only users with explicit consent can access private packages.
- In the event that a paid subscription is canceled, your packages will remain safe but will not be accessible until the subscription is renewed. The packages can be removed by deleting organization.

## Learn More

To stay updated on new features, best practices, and interesting uses of dartpm, follow us on [X](https://x.com/dartpmsupport).

For tutorials, user guides, and more, visit the [dartpm Docs](#).

## CLI Reference Documentation

While this documentation covers many aspects of using dartpm from the CLI, you can also access in-depth command line help through the `dartpm` CLI itself. You can get help for any command by running:

```bash
dartpm help
```
