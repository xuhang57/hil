# HIL Command Line Tool Guide

## Introduction
All HIL command line tool (CLI) should follow this guideline so we have a consistent structure for the tool. Please take a look at this guide when you are implementing a new command for the HIL CLI.

## Command Structure
HIL has a consistent and predictable CLI format for all of its commands.

Commands take the form:

```
hil <object> <sub-object> <action> [<command-arguments>]
```

> Note:
> <sub-object> sometimes are not necessary to a certain commands.

### Objects

The objects consist of one word to compose a unique name. Each object should have its commands in its own module file. Here is a list of objects currently we are supporting in HIL:

- user
- node
- project
- network
- switch
- port
- version
- networking-action

### Actions

The actions is to provide a consistent meaning to each other. Here is a list of actions:

- list
- show
- create
- connect
- delete
- detach
- register
- grant-access
- revoke-access
- show-console
- start-console
- stop-console
- add
- remove
- set-admin

### Command Entry Points

Commands are added to the HIL using `setuptools` entry points in `setup.py`.

