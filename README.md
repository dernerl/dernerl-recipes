# dernerl-recipes

[AutoPkg](https://github.com/autopkg/autopkg) recipes maintained by [@dernerl](https://github.com/dernerl).

| App | Recipes | Source | Code signature |
|---|---|---|---|
| [IceMelt](https://github.com/pnikolaidis/icemelt): menu bar manager for macOS 26+ | `IceMelt.download`, `IceMelt.munki` | Vendor Sparkle feed, GitHub Releases | Team ID `VZGXGAK29Q` |
| [Irrlicht](https://github.com/ingo-eichhorst/Irrlicht): Claude Code session lights in the macOS menu bar | `Irrlicht.download`, `Irrlicht.munki` | Vendor Sparkle feed, GitHub Releases | Team ID `93Y3GMJAMV` |

## Usage

```
autopkg repo-add dernerl-recipes
autopkg make-override IceMelt.munki
autopkg run -v IceMelt.munki MakeCatalogs.munki
```

The `.munki` recipe imports into the `testing` catalog. Adjust metadata such as the catalog or category in your override.

Please report broken recipes as an issue.
