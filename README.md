# devtoolkit

Small, dependency-free helpers for the kind of thing you end up rewriting in every
project: slugifying a title, truncating a string, splitting a list into fixed-size
batches.

Built collaboratively by [karandhaodiyal28-hash](https://github.com/karandhaodiyal28-hash)
and [devilsgamer70-lang](https://github.com/devilsgamer70-lang).

## Install

```bash
pip install -e .
```

## Usage

```python
from devtoolkit import chunk_list, slugify, truncate

slugify("Hello World!")            # -> "hello-world"
truncate("a very long sentence", 10) # -> "a very..."
chunk_list([1, 2, 3, 4, 5], 2)      # -> [[1, 2], [3, 4], [5]]
```

## CLI

```bash
devtoolkit slugify "Hello World!"     # hello-world
devtoolkit chunk 5 2                   # 0 1 | 2 3 | 4
```

## Development

```bash
python -m pip install -e .
python -m pytest tests -q
```

## License

MIT - see [LICENSE](LICENSE).
