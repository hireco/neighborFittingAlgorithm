## neighborFittingAlgorithm

An Energy prediction model of heterofullerenes by the neighbour atoms

### Directories in cage 
------------------------------------------------------

#### 1. caled
Directories of calculated structures,of which the sub-directories are listed as below,

```
CONTCAR  OSZICAR  OUTCAR  POSCAR  slurm.out
```


#### 2. data
Calculated data listed as below,

```
b.mat  branches.mat  enList  error  fitting  mini  myList.mat  top100  vectors.mat
```

#### 3. posFiles
POSCAR files

#### 4. tasks
Directories of calculated structures appended

#### hint
1. All files in cage and its sub-directories are for the purpose of demonstration.
2. If want to calculate a cage,for example, cage No. 937, first do as below,

```shell
mkdir 937
cd 937
mkdir caled data posFiles tasks
```

Then initialize the cage
```
./initFitting.sh 937
```

After cage initializing, do the iterations, for example from 1 to 5, do as below,
```
./loopFitting.sh 937 1 5
```

Do the last fitting
```
./finaFitting.sh 937 1 5
```


