# VoltaVision
*['Volta' from voltage + 'Vision' from visual data]*

VoltaVision is a lightweight CNN for classifying electronic components. It was pre-trained on different datasets and fine-tuned on our dataset (available under the Dataset directory). Through knowledge transfer, it was able to reach accuracies of over 90%, being on par with more common models such as ResNet-18 while being a fraction of the size.

# Video Demo

A video showcasing how VoltaVision could be used in a prototype electronic component lending machine.

https://github.com/AnasIshfaque/VoltaVision/assets/87610426/8ee3caab-aadf-4fd7-85eb-67362b91daa7

# Dataset
We took pictures of three distinct electronic components (Humidity sensor (DH11), Transistor and Bluetooth module) from different angles on a white background. There are over 100 images for each of the classes, totalling to 328 images. Here is what the distribution looks like:

| **Classes**      | **Instance** |
|------------------|--------------|
| Transistor       | 110          |
| Humidity Sensor  | 116          |
| Bluetooth Module | 102          |

# Reproducing Our Results

