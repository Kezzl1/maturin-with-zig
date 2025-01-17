

# install-pinned/maturin-with-zig

![](https://shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)

Securely install the latest [maturin[zig]](https://pypi.org/project/maturin/) release from PyPI.

This action installs a pinned version of **maturin[zig]** and all its dependencies,         making sure that file hashes match. Pinning your dependencies stops supply chain attacks where an adversary         replaces maturin[zig] or one of its dependencies with malicious code.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
      - name: Install maturin[zig] from PyPI
        uses: install-pinned/maturin-with-zig@da01cba93d4f50920a4a34aefba7acfda070c351  # 0.14.2
```

## Alternatives

This action is a relatively simple wrapper around the fantastic [pip-tools](https://pip-tools.rtfd.io)         and is most useful if there is no existing `requirements.txt`/`poetry.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [@install-pinned README](https://github.com/install-pinned) for details.
