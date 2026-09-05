# Matugen theming (fork only)

`fluidity.j2` is the [matugen](https://github.com/InioX/matugen) template that
generates `src/theme.css` (the `--m3-*` variables the "Matugen" theme in
`data.ts` reads). Fork-specific — not part of upstream.

Wire it up in `~/.config/matugen/config.toml`:

```toml
[templates.fluidity]
input_path  = "~/.config/matugen/templates/fluidity.j2"
output_path = "~/Documents/Development/fluidity/src/theme.css"
```

Regenerate on wallpaper change: `matugen image <path>`. `src/theme.css` is then
overwritten by matugen, so treat it as generated.
