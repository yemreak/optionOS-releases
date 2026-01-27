# optionOS Releases

Auto-update feed for optionOS.

## How it works

1. `appcast.xml` contains version info and download URLs
2. optionOS checks this feed for updates via Sparkle
3. DMG files are hosted in GitHub Releases

## For maintainers

When releasing a new version:

```bash
# In optionOS repo
make release
# This will:
# 1. Build and sign DMG
# 2. Upload to GitHub Releases
# 3. Update appcast.xml with signature
```
