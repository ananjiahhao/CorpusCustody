# Cookbook: gating a corpus before training

Run the gate before a dataset enters a training run, not after.

## 1. Check the manifest

```
python -m corpuscustody check samples/permissive.manifest
```

The report names each record, its license class, and its gate verdict. Exit
code 1 means a hold or a block; 2 means the manifest could not be parsed.

## 2. Explain a verdict

```
python -m corpuscustody explain samples/sharealike.manifest
```

Explain prints the obligation rows behind the verdict, which is what a review
needs when the answer is "hold, share-alike propagates".

## 3. Pin the provenance

Keep the manifest revision in the training run record. The gate prints the
fetch date and source revision with every verdict so the run is reproducible.

## 4. Put it in CI

The gate is offline and deterministic, so a CI step is enough:

```
python -m corpuscustody check manifests/dataset.manifest
```
