# coc-discord(-neovim?)

This is a fork of upstream `coc-discord` with refactorings and added features.

## What Features are Implemented Here

- Rich presences reports that the application being used is Neovim
- Large and small image assets in the rich presence based on open file.
-- Languages reported:
-- c, c++, java, typescript, javascript, python, yaml, html, css, php, ruby
- Ability to change runtime behaviors based on environment variables.
-- Environment variables:
-- `CLIENT_ID`
-- `ELAPSE_UPDATE_DURATION`
- Logging output to `:CocInfo`

## What Other Features are Planned

- Deriving the project root from `coc`'s built-in api.
- The ability to ignore showing sensitive projects.
- Setting logging levels (for development purposes).

## Running this Repository

Currently, this repository is not published on npm and must be installed
manually in a somewhat hacky way.

0. Run neovim.
1. Clone this repository.
2. Install `coc` via a plugin manager.
3. `CocInstall coc-discord`
4. Navigate to and delete: `$HOME/.cache/coc/node_modules/coc-discord`
5. `ln -s <location to this repo> $HOME/.cache/coc/node_modules/coc-discord`
6. Open or restart Discord.
7. Open neovim in the root of a project directory.

<!-- vim:tw=80:fo+=t
-->
