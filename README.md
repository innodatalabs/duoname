# duoname

Generate a two-word random name using the pattern `<adjective>-<noun>`.
Useful for generating user-friendly names and IDs.

No dependencies, easy to use.

## Usage

```python
from duoname import duoname

name = duoname()
```

## Building

```bash
pip install -e .[dev]
pip wheel . --no-deps
twine upload duoname-{version}-py3-none-any.whl -u __token__ -p {pypi-token}
```

## Credits

Word lists are taken from this wonderful repo: [`wordlists` (GitHub)](https://github.com/imsky/wordlists.git).

## FAQ

Q: Why not [`randomname` (GitHub)](https://github.com/beasteers/randomname)?

A: I really hate transient dependencies, and `randomname` package depends on `fire`.
