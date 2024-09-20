# U-Net for Electronic Devices Segmentation (TensorFlow implementation)

To build the model, I used the segmentation-models library, which was developed and made available on GitHub by Pavel Yakubovskiy (https://github.com/qubvel/segmentation_models?tab=readme-ov-file). The library was developed for Python and includes an implementation of neural networks for image segmentation based on Keras and TensorFlow. The main features of the segmentation-models library  are as follows:
o	it is a high-level interface that facilitates the construction of models;
o	includes 4 neural network architectures for binary and multiclass segmentation (U-Net, FPN, Linknet, PSPNet);
o	25 backbones are available for each architecture;
o	all backbones include pre-trained weights to achieve faster convergence of the training algorithm;
o	contains the implementation of segmentation losses (Jaccard, Dice, Focal) and segmentation quality metrics (IoU, F1-score).
To build the image segmentation model, I used the U-Net architecture with the EfficientNetB3 backbone. The training process consisted of 30 epochs, during which the learning rate was 1E-4. The dataset I prepared and used in this experiment can be downloaded from the Zenodo platform: https://doi.org/10.5281/zenodo.13786143. Sample images and their masks included in the dataset are show below. You can use the shared code for your own experiments with other neural network architectures available in the segmentation-models library  and various backbone networks.

![image](https://github.com/user-attachments/assets/a6f2ac13-2d6d-406b-9416-88a9a767885d)
