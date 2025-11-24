# Shell Command Argument Ordering

Avoid placing arguments before a subcommand,  which prevents matching permission patterns correctly—e.g., `Bash(git log:*)` won't match `git -C /path log`.

Where the argument cannot be made postfix, as with `git -C`, use an alternative such as `cd /path && git log`.
