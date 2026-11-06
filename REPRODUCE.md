# Reproducing this repository

Input: the Parquet files listed below, revision `fecc2c971945cacd914c63b54ee22db9149e58c9` of the `voilaj/swiss-caselaw` dataset
(`https://huggingface.co/datasets/voilaj/swiss-caselaw/resolve/fecc2c971945cacd914c63b54ee22db9149e58c9/<file>`), plus `graph/statute_references.parquet`
from the same revision, and lexifina/switzerland-law `main` for the overlay's `law_commit`.

```
python tools/build.py so <cache with data/ and graph/> <empty folder> --today 2026-11-06
```

Needs Python 3 and `duckdb`. Gives 13,667 decision commits and one documentation commit, hash for hash.

## SHA-256 of the input files

```
3ef5d7b17c5b5b190cdab16f8e4cfd2b21504c21d45297a1dd6f3f0bb9c86dd4 *so_gerichte.parquet
```
