# FastDD-Exp

## Datasets

Provided in datasets.zip, includes 14 datasets mentioned in our paper.

## Exp-1: DD discovery methods

We have implemented IE-Hybrid with our best efforts, and the code is available in [IE.zip](https://github.com/TristonK/FastDD-Exp/blob/main/Exp-1/IE.zip).

Additionally, we provide implementations for BF and TD-PO, packaged in [BF-TDPO.jar](https://github.com/TristonK/FastDD-Exp/blob/main/Exp-1/BF-TDPO.jar). You can customize the arguments to use different methods.

You can follow the instructions [here](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-1) to run IE-Hybrid, BF and TD-PO.

## Exp-2 RFD dicovery methods

We use Domino's thresholds to run FastDD and IE-Hybrid, threshold files are provided [here.](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-2)


You can modify the third parameter to use the threshold in the corresponding file. For example:
```shell
java -jar FastDD.jar ./FastDD-Exp/dataset/restaurant.csv -1 ./FastDD-Exp/Exp-2/thresholds/restaurant.txt
```
It will use all the data in `restaurant.csv` as input and select the data in `restaurant.txt` as the threshold for each attribute.

## Exp-3 Time decompostion

Our program outputs relevant information including the number of DDs and running time. We provide an output example [here.](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-3)

## Exp-4: Scalability of FastDD

Datasets varying |r| and |R| are provided in datasets.zip

## Exp-5: Comparison of methods to build diff-set

We use `Encoding` method in default.

Other two diff-set construction methods are implemented in:
- Naive: `src/main/java/bruteforce/DFSetCount.java`
- Bitset: `src/main/java/fastdd/dfset/BitSetISNBuilder.java`


## Exp-6: Speed-up ratio with parallelism

You can modify the number of threads in `Config.java`, Setting the value of `ThreadSize` can control the number of threads used .

## Exp-7: Ranking DDs

Three datasets' column description and its top20 DDs are provided in [Exp-7](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-7).

## Exp-8: DDs for duplicate identification

The restaurant dataset is available for download in [datasets.zip](https://github.com/TristonK/FastDD-Exp/blob/main/datasets.zip). To obtain an unlabeled version of the dataset, simply remove the "class" column.

You can get our Top20 DDs in [Exp-7](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-7)

## Exp-9: DDs for detecting inconsistencies

Datasets with noises, along with the corresponding indexes of violating tuples (starting at 0), are available in [Exp-9](https://github.com/TristonK/FastDD-Exp/tree/main/Exp-9)