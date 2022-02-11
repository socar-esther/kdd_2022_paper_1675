# kdd 2022 paper 1675
Implementation of "Discovering the Effectiveness of Pre-Training for Image Recognition in a Large-scale Car-sharing Platform"

## Datasets
We open our domain benchmark set in [URL](https://socar-kp.github.io/sofar_image_dataset/)

## How to run
- Run the upstream tasks
```shell
$ ./run_upstream.shs
```

- Run the downstream tasks (car-class classification, car-defect classification)
```shell
$ ./run_upstream.sh
```
- Run the CKA modules to check the layerwise similarity of the representations
```shell
$ python CKA-Centered-Kernel-Alignment/cka_main.py  # check the layerwise CKA 
$ python CKA-Centered-Kernel-Alignment/cka_lower_layer_higher.py # check the CKA of lower & higher layer
```
