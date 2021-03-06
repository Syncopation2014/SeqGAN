# SeqGAN

## Requirements: 
Tensorflow r0.10  
Cuda 7.5 (for GPU)  
nltk python package

## Introduction
We provide example codes to repeat the synthetic data experiments with oracle evaluation mechanisms.
Move to MLE SeqGAN folder and run
```
python pretrain experiment.py
```
will start maximum likelihood training with default parameters.
In the same folder, run
```
python sequence gan.py
```
will start SeqGAN training.
After installing nltk python package, move to pg_bleu folder and run
```
python pg bleu.py
```
will start policy gradient algorithm with BLEU score (PG-BLEU), where the final reward for MC search comes  
from a predefined score function instead of a CNN classifier.
Finally, move to schedule sampling folder and run
```
python schedule sampling.py
```
will launch SS algorithm with default parameters.
