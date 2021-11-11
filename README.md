# legacy-pi
Static package index for legacy packages unavailable elsewhere

## Updating the static pages with new packages

Run on the repository root:

```
dumb-pypi --package-list <(ls packages) \
    --packages-url https://raw.githubusercontent.com/renalreg/legacy-pi/packages \
    --output-dir .
```
