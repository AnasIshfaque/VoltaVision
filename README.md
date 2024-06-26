# VoltaVision
*['Volta' from voltage + 'Vision' from visual data]*

VoltaVision is a lightweight CNN for classifying electronic components. It was pre-trained on different datasets and fine-tuned on our dataset (available under the Dataset directory). Through knowledge transfer, it was able to reach accuracies of over 90%, being on par with more common models such as ResNet-18 while being a fraction of the size.

# Video Demo

A video showcasing how VoltaVision could be used in a prototype electronic component lending machine.

https://github.com/AnasIshfaque/VoltaVision/assets/87610426/8ee3caab-aadf-4fd7-85eb-67362b91daa7

**N.B:** In case the video here does not play, download the **Lending Machine demo.mp4**

# Dataset
We took pictures of three distinct electronic components (Humidity sensor (DH11), Transistor and Bluetooth module) from different angles on a white background. There are over 100 images for each of the classes, totalling to 328 images. Here is what the distribution looks like:

| **Classes**      | **Instance** |
|------------------|--------------|
| Transistor       | 110          |
| Humidity Sensor  | 116          |
| Bluetooth Module | 102          |

# Folder structure

```
Fine-tuning dataset/
├─ THB_dataset/
│  ├─ Bluetooth/
│  ├─ Humidity/
│  ├─ Transistor/
Lending Machine/
├─ LendTronics_Arduino_code.ino
├─ LendTronics_Py_code.ipynb
├─ database.sql
pretrained_models/
├─ best_CIFAR100_checkpoint.model
├─ best_CIFAR10_checkpoint.model
├─ best_CPR_dataset_checkpoint.model
├─ best_ECD_dataset_checkpoint.model
├─ best_EleComp_dataset_checkpoint.model
SOTA_ImageNet.ipynb
VoltaVision_CIFAR_10.ipynb
VoltaVision_Electronics.ipynb
VoltaVision_CIFAR_100.ipynb
```

# Experiments

- **SOTA_ImageNet.ipynb** contains the code and results for conducting transfer learning using State-Of-The-Art pretrained models
- **VoltaVision_CIFAR_10.ipynb** contains the code and results for conducting transfer learning using our VoltaVision pretrained on the CIFAR-10 dataset
- **VoltaVision_Electronics.ipynb** contains the code and results for conducting transfer learning using VoltaVision pretrained on Electronic datasets similar to the fine-tuning dataset
- **VoltaVision_CIFAR_100.ipynb** contains the code and results for conducting transfer learning using our VoltaVision pretrained on the CIFAR-100 dataset

# Pretrained models

It contains the saved model parameters for the 5 pretrained VoltaVision model using different training datasets.

# Citations

To cite VoltaVision in academic papers, please use the following BibTeX entry:

```
@inproceedings{
osmani2024voltavision,
title={VoltaVision: A Transfer Learning model for electronic component classification},
author={Anas Mohammad Ishfaqul Muktadir Osmani and Taimur Rahman and Salekul Islam},
booktitle={The Second Tiny Papers Track at ICLR 2024},
year={2024},
url={https://openreview.net/forum?id=JHTqFvmVYz}
}
```

Contact the author: aosmani203004@bscse.uiu.ac.bd, 
trahman221427@bscse.uiu.ac.bd
