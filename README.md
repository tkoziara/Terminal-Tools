# Terminal Tools

A collection of command-line utilities.

## screen_tt

Wrapper for GNU Screen with numbered session references.

```bash
screen_tt           # list sessions with numbers (1, 2, 3...)
screen_tt 1         # attach to session #1
screen_tt tail -50  # show last 50 lines from all sessions
screen_tt --help    # show usage
```

## git_update_tt

Quick git workflow: stage, commit, rebase, push.

```bash
git_update_tt                      # stage all, auto message
git_update_tt file.txt             # stage specific file(s)
git_update_tt -m "fix bug"         # custom commit message
git_update_tt -m "msg" src/        # custom message + stage path
git_update_tt -vim                 # open editor for commit message
git_update_tt --dry-run            # preview commands
```

Auto-generates commit messages like `"updated file1, file2"` unless `-m` or `-vim` is used.

Apache 2.0 License
