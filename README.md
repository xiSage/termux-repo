# termux-repo

Personal Termux APT repository hosted on GitHub Pages.

## Add the repository

Run in Termux:

```bash
echo "deb [trusted=yes] https://xisage.com/termux-repo stable main" \
  > $PREFIX/etc/apt/sources.list.d/xisage.list

pkg update
```

## Install packages

```bash
pkg install hitokoto
```

## Available packages

| Package | Description |
|---------|-------------|
| hitokoto | Hitokoto CLI - fetch a random hitokoto sentence in the terminal |

## Notes

- The repository is built and published automatically by the [hitokoto-cli](https://github.com/xiSage/hitokoto-cli) CI.
- `[trusted=yes]` is required since the repository is not GPG-signed.
