### Clone repository
``` 
git clone https://github.com/fsept11/FoolHD.git 
```
### Setup environment
```
conda create --name FoolHD --file requirements.txt
conda activate FoolHD 
```
### Usage
```
usage: main.py [-h] [-task {untargeted,targeted,bim,fgsm}] [-load_model]
               [-configuration CONFIGURATION] [-create_adversarial_examples]
               [-score_adversarial_examples] [--start START] [--end END]

optional arguments:
  -h, --help            show this help message and exit
  -task {untargeted,targeted,bim,fgsm}
                        Which task to run. (e.g. untargeted, tageted, bim,
                        fgsm)
  -load_model           Whether to load pre-trained model.
  -configuration CONFIGURATION
                        Configuration file - This file needs to be modified in order to accomodate for data path changes. 
  -create_adversarial_examples
  -score_adversarial_examples
  --start START         Dataset sample start index (0 first/-1 last) - Useful
                        to compute adversarial samples in parallel.
  --end END             Dataset sample end index (0 first/-1 last) - Useful to
                        compute adversarial samples in parallel.
```