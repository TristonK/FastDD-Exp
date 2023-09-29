# Exp-1 Against IE-Hybrid

## How To Run IE-Hybrid

1. Download our IE-Hybrid code in IE.zip
2. Building the project with maven, you can get `IE.jar`
3. Run IE.jar as follows:
```shell
java -jar IE.jar <fp> <rowLimit> <thresholds>
```

- `fp`: input file path.
- `threshold`: if you want to use specific thresholds, input filepath; Or we will sample the dataset and get thresholds.
- `rowLimit`: rows limit, using -1 or empty will use full dataset.