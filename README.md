<h2>Tensorflow-Image-Segmentation-RINGS-Prostate-Tumor (2024/12/25)</h2>

This is the first experiment of Image Segmentation for RINGS Prostate Tumor 
 based on 
the latest <a href="https://github.com/sarah-antillia/Tensorflow-Image-Segmentation-API">Tensorflow-Image-Segmentation-API</a>, 
and  <a href="https://drive.google.com/file/d/1hivmPx1lVm6fOc7QQwjjCP4vrQ3PVYZ1/view?usp=sharing">
RINGS-Prostate-Tumor-ImageMask-Dataset.zip</a>, which was derived by us from 
<a href="https://data.mendeley.com/datasets/h8bdwrtnr5/1">
<b>
RINGS algorithm dataset<br>
</b>
</a>
<br>
<hr>
<b>Actual Image Segmentation for Images of 1500x1500 pixels</b><br>
As shown below, the inferred masks look similar to the ground truth masks. <br>

<table>
<tr>
<th>Input: image</th>
<th>Mask (ground_truth)</th>
<th>Prediction: inferred_mask</th>
</tr>
<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_14_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_14_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_14_2.jpg" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_16_6.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_16_6.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_16_6.jpg" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_10_14_4.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_10_14_4.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_10_14_4.jpg" width="320" height="auto"></td>
</tr>
</table>

<hr>
<br>
In this experiment, we used the simple UNet Model 
<a href="./src/TensorflowUNet.py">TensorflowSlightlyFlexibleUNet</a> for this Prostate-TumorSegmentation Model.<br>
As shown in <a href="https://github.com/sarah-antillia/Tensorflow-Image-Segmentation-API">Tensorflow-Image-Segmentation-API</a>.
you may try other Tensorflow UNet Models:<br>

<li><a href="./src/TensorflowSwinUNet.py">TensorflowSwinUNet.py</a></li>
<li><a href="./src/TensorflowMultiResUNet.py">TensorflowMultiResUNet.py</a></li>
<li><a href="./src/TensorflowAttentionUNet.py">TensorflowAttentionUNet.py</a></li>
<li><a href="./src/TensorflowEfficientUNet.py">TensorflowEfficientUNet.py</a></li>
<li><a href="./src/TensorflowUNet3Plus.py">TensorflowUNet3Plus.py</a></li>
<li><a href="./src/TensorflowDeepLabV3Plus.py">TensorflowDeepLabV3Plus.py</a></li>

<br>

<h3>1. Dataset Citation</h3>
The dataset used here has been take from the following web site<br>

<a href="https://data.mendeley.com/datasets/h8bdwrtnr5/1">
<b>
RINGS algorithm dataset<br>
</b>
</a>

<br>
Published: 15 April 2021<br>
Version 1<br>
DOI:10.17632/h8bdwrtnr5.1<br>
<br>
<b>Contributors:</b><br>
Massimo Salvi, Martino Bosco, Luca Molinaro, Alessandro Gambella, Mauro Giulio Papotti,<br>
 Udyavara Rajendra Acharya, Filippo Molinari<br>
<br>
<b>Description</b><br>

This repository contains the image dataset and the manual annotations used to develop the RINGS algorithm for automated prostate glands segmentation:<br>
 Salvi M., Bosco M., L. Molinaro, Gambella A., Papotti M., Udyavara Rajendra Acharya, and Molinari F., <br>
"A hybrid deep learning approach for gland segmentation in prostate histopathological images", <br>
Artificial Intelligence in Medicine 2021 (DOI: 10.1016/j.artmed.2021.102076)
<br>
<br>
Background: In digital pathology, the morphology and architecture of prostate glands have been routinely adopted by pathologists to evaluate the presence of cancer tissue. The manual annotations are operator-dependent, error-prone and time-consuming. The automated segmentation of prostate glands can be very challenging too due to large appearance variation and serious degeneration of these histological structures.
Method: A new image segmentation method, called RINGS (Rapid IdentificatioN of Glandural Structures), is presented to segment prostate glands in histopathological images. We designed a novel glands segmentation strategy using a multi-channel algorithm that exploits and fuses both traditional and deep learning techniques. Specifically, the proposed approach employs a hybrid segmentation strategy based on stroma detection to accurately detect and delineate the prostate glands contours.
Results: Automated results are compared with manual annotations and seven state-of-the-art techniques designed for glands segmentation. Being based on stroma segmentation, no performance degradation is observed when segmenting healthy or pathological structures.  Our method is able to delineate the prostate gland of the unknown histopathological image with a dice score of 90.16% and outperforms all the compared state-of-the-art methods.
Conclusions: To the best of our knowledge, the RINGS algorithm is the first fully automated method capable of maintaining a high sensitivity even in the presence of severe glandular degeneration. The proposed method will help to detect the prostate glands accurately and assist the pathologists to make accurate diagnosis and treatment. The developed model can be used to support prostate cancer diagnosis in polyclinics and community care centres. 
<br><br>
<b>Licence</b>: CC BY 4.0<br>


<br>
<h3>
<a id="2">
2 Prostate-Tumor ImageMask Dataset
</a>
</h3>
 If you would like to train this Prostate-Tumor Segmentation model by yourself,
 please download the dataset from the google drive  
<a href="https://drive.google.com/file/d/1hivmPx1lVm6fOc7QQwjjCP4vrQ3PVYZ1/view?usp=sharing">
RINGS-Prostate-Tumor-ImageMask-Dataset.zip</a>
, expand the downloaded ImageMaskDataset and put it under <b>./dataset</b> folder to be
<pre>
./dataset
└─Prostate-Tumor
    ├─test
    │   ├─images
    │   └─masks
    ├─train
    │   ├─images
    │   └─masks
    └─valid
        ├─images
        └─masks
</pre>
This is a 512x512 pixels sub dataset generated from 1500x1500 pixels IMAGES and MANUAL_TUMOR of TRAIN only.<br>
We excluded all black (empty) masks and their corresponding images to generate our dataset from the original one.<br>  
<pre>
./RINGS
└─TRAIN
    ├─IMAGES
    └─MANUAL TUMOR
</pre>
>
<br>
<b>Prostate-Tumor Statistics</b><br>
<img src ="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/Prostate-Tumor_Statistics.png" width="512" height="auto"><br>
<br>
As shown above, the number of images of train and valid datasets is not enough to use for a training set of our segmentation model.
<br>
<br>
<b>Train_images_sample</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/train_images_sample.png" width="1024" height="auto">
<br>
<b>Train_masks_sample</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/train_masks_sample.png" width="1024" height="auto">
<br>

<h3>
3 Train TensorflowUNet Model
</h3>
 We have trained Prostate-Tumor TensorflowUNet Model by using the following
<a href="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/train_eval_infer.config"> <b>train_eval_infer.config</b></a> file. <br>
Please move to ./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumorand run the following bat file.<br>
<pre>
>1.train.bat
</pre>
, which simply runs the following command.<br>
<pre>
>python ../../../src/TensorflowUNetTrainer.py ./train_eval_infer.config
</pre>
<hr>

<b>Model parameters</b><br>
Enabled Batch Normalization.<br>

Defined a small <b>base_filters=16</b> and large <b>base_kernels=(9,9)</b> for the first Conv Layer of Encoder Block of 
<a href="./src/TensorflowUNet.py">TensorflowUNet.py</a> 
and a large num_layers (including a bridge between Encoder and Decoder Blocks).
<pre>
[model]
normalization  = True
base_filters   = 16
base_kernels   = (9,9)
num_layers     = 7
dilation       = (1,1)
</pre>

<b>Learning rate</b><br>
Defined a small learning rate.  
<pre>
[model]
learning_rate  = 0.0002
</pre>

<b>Online augmentation</b><br>
Disabled our online augmentation tool. 
<pre>
[model]
model         = "TensorflowUNet"
generator     = False
</pre>

<b>Loss and metrics functions</b><br>
Specified "bce_dice_loss" and "dice_coef".<br>
<pre>
[model]
loss           = "bce_dice_loss"
metrics        = ["dice_coef"]
</pre>
<b >Learning rate reducer callback</b><br>
Enabled learing_rate_reducer callback, and a small reducer_patience.
<pre> 
[train]
learning_rate_reducer = True
reducer_factor     = 0.4
reducer_patience   = 4
</pre>


<b>Early stopping callback</b><br>
Enabled early stopping callback with patience parameter.
<pre>
[train]
patience      = 10
</pre>

<b>Epoch change inference callbacks</b><br>
Enabled epoch_change_infer callback.<br>
<pre>
[train]
epoch_change_infer       = True
epoch_change_infer_dir   =  "./epoch_change_infer"
epoch_changeinfer        = False
epoch_changeinfer_dir    = "./epoch_changeinfer"
num_infer_images         = 1
</pre>

By using this callback, on every epoch_change, the inference procedure can be called
 for 6 images in <b>mini_test</b> folder. This will help you confirm how the predicted mask changes 
 at each epoch during your training process.<br> <br> 

<b>Epoch_change_inference output</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/epoch_change_infer.png" width="1024" height="auto"><br>
<br>

In this experiment, the training process was stopped at epoch 37  by EarlyStopping Callback.<br><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/train_console_output_at_epoch_37.png" width="720" height="auto"><br>
<br>

<a href="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/eval/train_metrics.csv">train_metrics.csv</a><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/eval/train_metrics.png" width="520" height="auto"><br>

<br>
<a href="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/eval/train_losses.csv">train_losses.csv</a><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/eval/train_losses.png" width="520" height="auto"><br>

<br>

<h3>
4 Evaluation
</h3>
Please move to a <b>./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor</b> folder,<br>
and run the following bat file to evaluate TensorflowUNet model for Prostate-Tumor.<br>
<pre>
./2.evaluate.bat
</pre>
This bat file simply runs the following command.
<pre>
python ../../../src/TensorflowUNetEvaluator.py ./train_eval_infer_aug.config
</pre>

Evaluation console output:<br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/evaluate_console_output_at_epoch_37.png" width="720" height="auto">
<br><br>Image-Segmentation-Prostate-Tumor

<a href="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/evaluation.csv">evaluation.csv</a><br>

The loss (bce_dice_loss) to this Prostate-Tumor/test was not low, and dice_coef not so high as shown below.
<br>
<pre>
loss,0.3912
dice_coef,0.6951</pre>
<br>

<h3>
5 Inference
</h3>
Please move to a <b>./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor</b> folder<br>
,and run the following bat file to infer segmentation regions for images by the Trained-TensorflowUNet model for Prostate-Tumor.<br>
<pre>
./3.infer.bat
</pre>
This simply runs the following command.
<pre>
python ../../../src/TensorflowUNetInferencer.py ./train_eval_infer_aug.config
</pre>
<hr>
<b>mini_test_images</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/mini_test_images.png" width="1024" height="auto"><br>
<b>mini_test_mask(ground_truth)</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/mini_test_masks.png" width="1024" height="auto"><br>

<hr>
<b>Inferred test masks</b><br>
<img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/asset/mini_test_output.png" width="1024" height="auto"><br>
<br>
<hr>
<b>Enlarged images and masks </b><br>

<table>
<tr>
<th>Image</th>
<th>Mask (ground_truth)</th>
<th>Inferred-mask</th>
</tr>

<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_15_1.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_15_1.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_15_1.jpg" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_14_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_14_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_14_2.jpg" width="320" height="auto"></td>
</tr>

<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_14_8.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_14_8.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_14_8.jpg" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_15_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_15_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_15_2.jpg" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_9_16_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_9_16_2.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_9_16_2.jpg" width="320" height="auto"></td>
</tr>
<tr>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/images/P5_D5_10_14_4.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test/masks/P5_D5_10_14_4.png" width="320" height="auto"></td>
<td><img src="./projects/TensorflowSlightlyFlexibleUNet/Prostate-Tumor/mini_test_output/P5_D5_10_14_4.jpg" width="320" height="auto"></td>
</tr>
</table>
<hr>
<br>


<h3>
References
</h3>
<b>1. RINGS algorithm dataset</b><br>
Massimo Salvi, Martino Bosco, Luca Molinaro, Alessandro Gambella, Mauro Giulio Papotti,<br>
 Udyavara Rajendra Acharya, Filippo Molinari<br>
DOI:10.17632/h8bdwrtnr5.1<br>

<a href="https://data.mendeley.com/datasets/h8bdwrtnr5/1">
https://data.mendeley.com/datasets/h8bdwrtnr5/1</a>
<br>


