![thumb-image](./images/android-chrome-192x192.png) 

Commit Messages Convention (CMC)
===

Commit Messages Convention (CMC) is designed to support GIT or SVN projects for better organization of the files that are versioned in the repository, we must insert comments preceded by the actions that were performed on the versioned files. This way the source code versioning is more flexible and cohesive, making it easier to identify what was done.

## How to use
By default, each action should be enclosed in brackets preceded by what was performed clearly and objectively during code versioning.

## Actions

The options below represent options that can be used at the beginning of each commit.

|Actions    |Description|
|:-:	      |:-:	    |
|[ADD]      | Used for when files are added to the project|
|[REMOVE]   | Used to signal file removal|
|[MOVE]     | Used when a file is moved from one directory to another.|
|[UPDATE]   | Used to enhance an existing file|
|[REFACTOR] | Used for source code refactoring|
|[PATCH]    | Used to represent routines for interim fixes.|
|[FIX]      | Used to represent Error / Fault Correction, identified by the manager or team working on the source code|
|[MERGE]    | Used when file merge is performed|
|[RENAME]   | Used when a file is renamed.|

## Usage

### Default Message
```
[ADD] Definition of xyz Files
```

### Title and Description
```
[UPDATE] Payment using cards

Creation of functionality that allows you to make payments using the XPTO flag credit card.
```

### Logging messages to modules

If **modules** and **functionality** are used, use the pattern `[action] module / functionality:` preceded by a brief description.

```
[FIX] Module/Feature: Description

Describing what was done in this fix.
```

## How NOT to use

It is not good practice to group multiple actions in the same commit. It is recommended that commits be linked to action.

```
[UPDATE/FIX] Description of the change and correction.
```

## Languages
- [PT-BR](./Readme-Pt-BR.md)
