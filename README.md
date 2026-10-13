# kuro extensions

The extension registry of [kuro](https://github.com/ArieqAqila/kuro-ide): one folder per extension, each with a `kuro-ext.toml` (data only: language
definitions, nothing is ever executed) and a README.

```fish
kuro ext install ksystem                      # an extension of this registry, by name
kuro ext install https://github.com/you/your-extension@v1.0   # or any git repository with a kuro-ext.toml at its root
kuro ext list
```

kuro shows what it downloaded and asks before it installs (`--yes` skips the question). Extensions stored here are *not* part of the kuro repository,
so kuro stays small however many there are. See kuro's `docs/EXTENSIONS.md` for the manifest format.

| Folder | What |
|---|---|
| `ksystem/` | The ksystem screen definition language |

To add one: a new folder with a `kuro-ext.toml` and a README, and a line in the table above.
