# `@deepest-lore/cli` [![Travis](https://img.shields.io/travis/deepest-lore/cli.svg)](https://travis-ci.org/deepest-lore/cli) [![License](https://img.shields.io/github/license/deepest-lore/cli.svg)](license) [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdeepest-lore%2Fcli.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdeepest-lore%2Fcli?ref=badge_shield) [![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg)](https://renovatebot.com/) [![npm](https://img.shields.io/npm/v/@deepest-lore/cli.svg)](https://www.npmjs.com/package/@deepest-lore/cli) [![npm type definitions](https://img.shields.io/npm/types/@deepest-lore/cli.svg)](https://www.npmjs.com/package/@deepest-lore/cli)

A command-line tool for processing deepest-lore schemas and data.

All runs include a pass by [@deepest-lore/validator](https://www.npmjs.com/package/@deepest-lore/validator).

Warnings will be printed but do not count as an error by default.

## Parameters

### `--fs-import {path}`

The base directory from which to import; runs once then stops.  Exits on error
and returns a non-zero exit code.

Uses [@deepest-lore/fs-import](https://www.npmjs.com/package/@deepest-lore/fs-import).

### `--fs-import-watch {path}`

The base directory from which to import; runs once then waits for changes before
running again until terminated by the user.  Aborts run but does not exit on
error.

Uses [@deepest-lore/fs-import-watch](https://www.npmjs.com/package/@deepest-lore/fs-import-watch).

### `--warnings-as-errors`

When present, any warnings generated by
[@deepest-lore/validator](https://www.npmjs.com/package/@deepest-lore/validator)
will instead be treated as errors.  The standard error handling logic will then
apply.

### `--html-export {path}`

The base directory to which to export; this will be deleted and replaced with a
new directory containing the exported HTML.

Uses [@deepest-lore/html-export](https://www.npmjs.com/package/@deepest-lore/html-export).

## License

[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdeepest-lore%2Fcli.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdeepest-lore%2Fcli?ref=badge_large)
