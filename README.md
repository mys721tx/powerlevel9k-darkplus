# Powerlevel9k Darkplus

By [Yishen Miao](https://github.com/mys721tx)

## Description

A dark plus color theme for
[Powerlevel9k](https://github.com/bhilburn/powerlevel9k), Heavily influenced by
[vim-code-dark](https://github.com/tomasiser/vim-code-dark).

Works with [Powerlevel10k](https://github.com/romkatv/powerlevel10k) too.

## Usage

### With zplugin

```zsh
...
# Use a custom function to pass more options.
_config_powerline_custom() {
        POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(
                context
                dir
                dir_writable
                vcs
        )

        POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(
                status
                root_indicator
                background_jobs
                history
        )

        POWERLEVEL9K_SHORTEN_DIR_LENGTH=1
}

zplugin light mys721tx/powerlevel9k-darkplus
zplugin ice atinit"_config_powerline;_config_powerline_custom"
zplugin light romkatv/powerlevel10k
...
```

## License

[GNU General Public License, version 3](http://www.gnu.org/licenses/gpl-3.0.html)
