# DotConfig

Programming workspace setups. Similar to https://github.com/SOF3/nvim-config.

# Sublime Text

**Note: Vintage Command Mode refers to the Vim Normal Mode.**

## Global

| Feature                                    |                                       Hotkey                                       |                      Driven Plugin                       |
| ------------------------------------------ | :--------------------------------------------------------------------------------: | :------------------------------------------------------: |
| Vim like keys set with some customizations |                                         -                                          |     [Vintage](https://github.com/sublimehq/Vintage)      |
| Open sidebar                               |                          <kbd>Command</kbd>+<kbd>`</kbd>                           |                            -                             | - [x] Open sidebar: |
| Open a terminal tab                        |                          <kbd>Command</kbd>+<kbd>O</kbd>                           | [Terminus](https://packagecontrol.io/packages/Terminus)  |
| Open to current file#line on GitHub        |                          <kbd>Command</kbd>+<kbd>\\</kbd>                          | [GitHubinator](https://github.com/ehamiter/GitHubinator) |
| Go to code definition                      | Vintage Command Mode: <kbd>Shift</kbd>+<kbd>K</kbd>, <kbd>Shift</kbd>+<kbd>K</kbd> |                       Per language                       |
| Go to next problem in file                 | Vintage Command Mode: <kbd>Shift</kbd>+<kbd>K</kbd>, <kbd>Shift</kbd>+<kbd>M</kbd> |        [SublimeLinter](http://sublimelinter.com/)        |

## PHP

| Feature                            |                                       Hotkey                                       |                                        Driven Plugin                                         |                                                                                  Driver File                                                                                   |
| ---------------------------------- | :--------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Code linting                       |                    <kbd>Command</kbd>+<kbd>S</kbd> _(on save)_                     | [SublimeLinter-contrib-phpstan](https://github.com/Rockstar04/SublimeLinter-contrib-phpstan) |                                $PATH/[phpstan](https://github.com/Endermanbugzjfc/DotConfig/blob/master/sublime-text/Packages/User/phpstan.sh)                                 |
| Code standard fixing               |                    <kbd>Command</kbd>+<kbd>S</kbd> _(on save)_                     |                    [Phpcs](https://github.com/benmatselby/sublime-phpcs)                     |                                                                  $COMPOSER_HOME/vendor/bin/php-cs-fixer.phar                                                                   |
| Import class of the caret position | Vintage Command Mode: <kbd>Shift</kbd>+<kbd>K</kbd>, <kbd>Shift</kbd>+<kbd>J</kbd> |               [PHP Companion](https://github.com/erichard/SublimePHPCompanion)               | vendor/\* _(please disable [`index_exclude_gitignore`](https://github.com/Endermanbugzjfc/DotConfig/blob/master/sublime-text/Packages/User/Preferences.sublime-settings#L25))_ |
| Go to class function definition:   |                                   Same as global                                   |                                              -                                               | vendor/\* _(please disable [`index_exclude_gitignore`](https://github.com/Endermanbugzjfc/DotConfig/blob/master/sublime-text/Packages/User/Preferences.sublime-settings#L25))_ |

## Go

| Feature                                   |                   Hotkey                    |                                       Driven Plugin                                       |     Driver File      |
| ----------------------------------------- | :-----------------------------------------: | :---------------------------------------------------------------------------------------: | :------------------: |
| go.mod / go.sum files syntax highlighting |                      -                      |                    [Gomod](https://github.com/mitranim/sublime-gomod)                     |          -           |
| Code linting                              | <kbd>Command</kbd>+<kbd>S</kbd> _(on save)_ | [SublimeLinter-golangcilint](https://github.com/SublimeLinter/SublimeLinter-golangcilint) | $GOBIN/golangci-lint |
| Code formatting                           | <kbd>Command</kbd>+<kbd>S</kbd> _(on save)_ |                     [GoFmt](https://github.com/noonat/sublime-gofmt)                      |  $GOROOT/goimports   |
| Go function definition                    |               Same as global                |                        [GoGuru](http://alvarolm.github.io/GoGuru)                         |     $GOBIN/guru      |