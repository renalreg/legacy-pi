# legacy-pi
Static package index for legacy packages unavailable elsewhere

## Web interface

See https://renalreg.github.io/legacy-pi/

## Usage

### requirements.txt

Add the following to your requirements.txt:

```
--extra-index-url https://renalreg.github.io/legacy-pi/simple/simple/
```

### setup.py

Pass the argument to your `setup` function:

```python
    dependency_links=[
        'https://renalreg.github.io/legacy-pi/simple/simple/'
    ]
```

## Updating the static pages with new packages

Run on the repository root:

```
dumb-pypi --package-list <(ls packages) \
    --packages-url https://raw.githubusercontent.com/renalreg/legacy-pi/packages \
    --output-dir .
```
