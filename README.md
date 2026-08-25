# oliver-kriska/homebrew-tap

Homebrew formulae for my own tools.

```bash
brew tap oliver-kriska/tap
brew install oliver-kriska/tap/<formula>
```

## Formulae

### cmux-sentinel

An opinionated [cmux](https://cmux.com) sidebar: agent-state rows (⚡ working, ⏳ compacting,
❓ waiting on you) and AI usage meters for Claude, Codex and Amp.
Source: [oliver-kriska/cmux-sentinel](https://github.com/oliver-kriska/cmux-sentinel).

```bash
brew install oliver-kriska/tap/cmux-sentinel
cmux-sentinel deploy    # installs into ~/bin and ~/.config, wires launchd + cmux
cmux-sentinel doctor    # confirm the pipeline
```

`deploy` is needed after every `brew upgrade` too: Homebrew owns the files under its own prefix,
but the launchd agents run the copies in `~/bin`.

The formulae here are generated from each project's release tag — send changes to the source repo,
not to this one.
