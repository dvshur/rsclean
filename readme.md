# rscleanup

Utility for reclaiming disk space by removing `target` directories in Rust projects.

## Installation

Copy the script into your `$PATH`, for example:

```sh
curl -o ~/.local/bin/rsclean https://raw.githubusercontent.com/dvshur/rsclean/main/rsclean
chmod +x ~/.local/bin/rsclean
```

Ensure `~/.local/bin` is in your `$PATH`:

```sh
export PATH="$HOME/.local/bin:$PATH"
```

## Usage

```sh
rscleanup             # delete all ./**/target directories
rscleanup --dry       # show total size without deleting
rscleanup --exclude ./some/path/target [--exclude ./another/target ...]
                      # skip specific target directories
rscleanup --dry --exclude ./lib1/target
```
