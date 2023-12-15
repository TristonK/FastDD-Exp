# Exp-1 Against IE-Hybrid

## How To Run IE-Hybrid

1. Download our IE-Hybrid code in [IE.zip](https://github.com/TristonK/FastDD-Exp/blob/main/Exp-1/IE.zip)
2. Building the project with maven, you can get `IE.jar`
3. Run IE.jar as follows:
```shell
java -jar IE.jar <fp> <rowLimit> <thresholds>
```

- `fp`: input file path.
- `threshold`: if you want to use specific thresholds, input filepath; Or we will sample the dataset and get thresholds.
- `rowLimit`: rows limit, using -1 or empty will use full dataset.

## How To Run TDPO or BF

Run BF-TDPO.jar as follows:

```shell
java -jar BF-TDPO.jar <fp> <rowLimit> <thresholds> <method>
```

- `fp`: input file path.
- `threshold`: if you want to use specific thresholds, input filepath; Or we will sample the dataset and get thresholds.
- `rowLimit`: rows limit, using -1 or empty will use full dataset.
- `method`: using 0 to use BF, using 1 to use TD-PO 