# Yuval's helpers for Klotho development

These scripts are meant to help while working on [Klotho][1] itself. They are _not_ intended for help with working on Klotho-annotated projects.

## Installation

Clone this directory and add it to your `PATH` in your `~/zshrc`, `~/.bash_profile`, or similar.

## What's here

### klotho-use

Lets you easily switch between local and release versions of Klotho. For now, we only support two options:

- `klotho-use release [latest]` to use the release version of Klotho (provide the extra "latest" arg to also download the latest)
- `klotho-use local/dev` to use a local version; requires that you have `go` installed.

Future improvements could be to support multiple release versions, or multiple local dirs.

### pulumi-login

Lets you easily switch your pulumi login creds. Useful if you have access to both a personal account and a team account.

## pulumi-nuke

`pulumi down`s a stack, and optionally `rm`s it, without you having to actually have the stack locally. You just give it a fully qualified stack name, and it does the rest.

As a convenience, you can even just give it the URL to the ack at app.pululmi.com.

[1]: https://github.com/klothoplatform/klotho
