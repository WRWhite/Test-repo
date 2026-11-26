# Copilot Instructions

## Repository purpose

This is a small training repository for Git and Google's `repo` manifest utility. It does not contain an application build or package, and it has no automated test or lint suite.

The main artifact is `default.xml`, a `repo` manifest that defines:

- a `WRWhite` remote whose fetch base is `https://github.com/WRWhite`
- the `Test-repo` project at the `Test-repo` checkout path on the `main` revision
- the `ScratchPad` project at the `ScratchPad` checkout path on a pinned commit
- a default parallel sync setting of `sync-j="2"`

The README.md includes both repository clone commands and the manifest purpose. Keep these descriptions aligned when manifest project names, paths, revisions, remotes, or the sync setting change.

## Build, test, and lint

There are no build, test, or lint commands in this repository.

For the same kind of top-level validation available here, clone the repository with:

```sh
git clone https://github.com/WRWhite/Test-repo.git
```

Initialize a checkout using this manifest repository with the documented command:

```sh
repo init https://github.com/WRWhite/Test-repo
```

There is no single-test command.

## Manifest conventions

- Keep `default.xml` as valid XML and preserve the UTF-8 declaration and manifest structure.
- Do not place XML comments inside `default.xml`; the README records that comments are not supported.
- Put explanatory annotations for manifest entries in `README.md`, not in `default.xml`.
- Preserve attribute syntax for manifest elements; project entries require `remote`, `name`, `path`, and `revision`.
- When changing a project revision, use the intended branch, tag, or full commit hash consistently.
- Keep project paths free of comments or additional XML text so the manifest remains directly consumable by `repo`.
