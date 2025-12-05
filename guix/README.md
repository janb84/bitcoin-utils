# Guix Utilities

Tools for working with [Guix builds](https://github.com/bitcoin/bitcoin/blob/master/contrib/guix/README.md) of Bitcoin Core.

## `guix-shasums.sh`

A script for formatting the SHA256 checksums of Guix build outputs. Useful for pull-request reviews. 

**Usage:**
```shell
./guix/guix-shasums.sh [OPTIONS]
```

**Options:**
| Option | Description |
|--------|-------------|
| `-m, --markdown [FILE]` | Output in markdown format (optionally to a file) |
| `-c, --commit HASH` | Use a specific git commit hash instead of HEAD |
| `-h, --help` | Show help message |

**Example:**
```shell
# Generate checksums in markdown format
./guix/guix-shasums.sh -m

# Generate checksums for a specific commit
./guix/guix-shasums.sh -c abc123def456
```