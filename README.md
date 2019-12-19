![thumb-image](./images/android-chrome-192x192.png) 

Commit Messages Convention (CMC)
===

Commit Messages Convention (CMC) is designed to help **GIT** or **SVN** projects to a better organization of commits in the repository.
It defines that commenting must be preceded by the types of actions that were performed on versioned files.
This makes source code versioning more flexible and cohesive, making it easier to identify what has been done.

This convention follows [SemVer](http://semver.org/), describing features, fixes, and modifications that break compatibility in commit messages. 

## Specification
The keywords `MUST`, `MUST NOT`, `REQUIRED`, `SHALL`, `SHALL NOT`, `SHOULD`, `SHOULD NOT`, `RECOMMENDED`, `MAY` and `OPTIONAL` in this document are to be interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).

## How to use
By default, each type MUST be capitalized, in brackets, preceding what was done clearly and objectively during code versioning.

The commit message MUST be structured as follows:

```
[TYPE required] <description|header required>
--blank line--
<optional body>
--blank line--
<optional footer>
```
##### The message:
- MUST start with a `[TYPE]`
- `[TYPE]` MUST be uppercase, enclosed in brackets, followed by a space
- MUST contain a `<description>` after `[TYPE]`
- MAY contain `<body>` and/or `<footer>`
- MUST contain a `--blank line--` after `<description>` if you have `<body>`
- MUST contain a `--blank line--` after `<body>` if it has `<footer>`

### Types
The types below represent options that can be used at the beginning of each commit.

| Type      | Description |
|:-:        | :-: |
|`[FEAT]`     | When a new feature was developed |
|`[FIX]`      | When a feature/bug has been fixed |
|`[UPDATE]`   | When static files have been renamed, removed, moved from one directory to another, added or replaced |
|`[REFACTOR]` | When a code change that doesn't fix a bug nor add a feature |
|`[DOCS]`     | Documentation changes only |

### Special Types
Is RECOMMENDED that special types to use in conjunction with previous types, however, they MAY be used anywhere in the message.

| Type                              | Description |
|:-:                                | :-: |
|`[WIP]`                            | When a development is still in progress |
|`[BREAKING]` or `[BREAKING CHANGE]`| When commit includes a modification that breaks compatibility. MAY be used anywhere in commit (`<description>`, `<body>` or `<footer>`) |

#### Examples:
```
[FEAT][WIP] Introduces a new payment method
```
```
[FIX][BREAKING] Replaces PayPal Gateway with PayPal
```

### Description
For the commit `<description>` and `<body>` message, use the ["Commit Message Guide"](https://github.com/RomuloOliveira/commit-messages-guide/blob/master/README_en.md) pattern @RomuloOliveira, which basically consists of:
- **Use imperative**: The message from commit tells you what it does, not what it was **done**.
- **First letter in upper case**: because this is how you start a sentence in any text.
- **Try to communicate what commit does without having to look at the commit content.**

### Body
- **Use the body message to explain "why", "for what", "how", and additional details.**
- **Avoid commits with generic messages or no context.**
- **Try to limit the number of message columns:** We recommend 50 characters for the <description> and around 72 for the <body>.
- **Maintain language consistency:** Choose a language and stick to it.

### Footer
A `<footer>` of one or more lines MAY be provided after a `--blank line--` after `<body>`.
The `<footer>` MUST contain additional information about commit, eg issue/task number, pull-requests, proofreaders, modifications that break compatibility, with one additional information per line.

#### Examples
```
[FIX] Fix the method call "getProducts"

The expected return of the "getProducts" method was an array, but returned an object, 
which caused an error in production.

Fix issue #92
```

```
[FEAT][WIP] Creates the PayPalGateway Class

Creates the basic framework for PayPal integration, as well as the Gateway interface 
for future use.
```

```
[REFACTOR] Refactors the PagSeguro class

Rewrote of the PagSeguroGateway class to fit the Gateway interface standard.
```
```
[BREAKING CHANGE] Because the PagSeguroGateway class has been refactored, all methods have also been modified.

Depends on commit sd5f54s
```

```
[UPDATE] Add CSS files and images

Add missing files to assets/ directory
```

## Languages
- [PT-BR](./README-pt_BR.md)

## References
- [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)
- [Conventional Commits](https://www.conventionalcommits.org/pt-br/)
- [Commit Messages Guide](https://github.com/RomuloOliveira/commit-messages-guide)
- [Angular Commit Message Guidelines](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)