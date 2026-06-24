

## A very normal Fastfetch config made at 3 AM after finals.

### Preview

Displays:

* OS
* Kernel
* Uptime
* CPU
* GPU
* Memory
* Swap
* Shell
* Terminal
* Root disk usage
* DingusNux disk usage
* NVME disk usage
* Local IP

Image preview in repo

## Installation

If Fastfetch can't find your config, it is usually located at:

```bash
~/.config/fastfetch/config.jsonc
```

Simply:

1. Open your Fastfetch config.
2. Delete the existing contents (optional).
3. Copy and paste this repository's `config.jsonc`.
4. Save.
5. Run:

```bash
fastfetch
```

Done.

## Requirements

The logo path is currently set to my file path:

```bash
/mnt/DingusNux/Medias/memes/pyroman.txt
```

You will need to replace this with your own ASCII file.

```jsonc
"logo": {
    "source": "/path/to/your/ascii.txt"
}
```

## Troubleshooting

### Fastfetch not using the config

Check:

```bash
fastfetch --list-config-paths
```

### Config missing

Generate a fresh one:

```bash
mkdir -p ~/.config/fastfetch
fastfetch --gen-config > ~/.config/fastfetch/config.jsonc
```

Then paste the repository contents into the generated file.

### Pyro missing

Skill issue

Replace:

```jsonc
"source": "/mnt/DingusNux/Medias/memes/pyroman.txt"
```

with ur own path
