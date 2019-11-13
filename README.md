Code Versioning Standard (CVS)
===

For better organization of the files that are versioned in the repository, we must insert comments preceded by the actions that were performed on the versioned files. This way the source code versioning is more flexible and cohesive, making it easier to identify what was done.

## How to use
By default, it should be enclosed in square brackets, the type of action used to version files, and more than one action can be used in versioning code. Then, if applicable, indicate module / functionality and a colon; Finally, describe in a brief comment what was accomplished.

## Actions
- [ADD] Used for when files are added to the project;
- [REMOVE] Used to signal file removal;
- [MOVE] Used when a file is moved from one directory to another.
- [UPDATE] Used to enhance an existing file;
- [REFACTOR] Used for source code refactoring
- [PATCH] Used to represent routines for interim fixes.
- [FIX] Used to represent Error / Fault Correction, identified by the manager or team working on the source code;
- [MERGE] Used when file merge is performed;
- [RENAME] Used when a file is renamed.

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

### Modular Messages
```
[FIX] Module / FunctionName

Describing what was done in this fix.
```

### Action Grouping
```
[UPDATE/FIX] Description of the change and correction.
```
