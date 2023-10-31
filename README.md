# Circle of Wilis segmentation challenge (TopCow) MICCAI 2023
Our Model: 

We used nnU-Net with modified loss and got the 3rd rank in the final phase of Binary Segmentation of the Circle of Willis with MRA. For more details, please read the pdf file as uploaded. 

Results: 
Mean CoWclass Dice: 0.9537 ± 0.022
Mean clDice: 0.9818 ± 0.0193
Betti-0 Error: 0.8857 ± 0.8668

# Inference

1- Install nnU-Net from the original repository (https://github.com/MIC-DKFZ/nnUNet), or the code we shared here. </br>
2- Download the trained models via the link: https://drive.google.com/drive/folders/1a0n_kvpJbheSI6vEiilzea_OgezxnklS?usp=drive_link </br>
3- Copy the test images to "nnUNet_raw_data_base/nnUNet_raw_data/Task101_SCGM/imagesTs" and run the code:</br>
!nnUNet_predict -i nnUNet_raw_data_base/nnUNet_raw_data/Task101_SCGM/imagesTs -o nnUNet_Prediction_Results/Task101_SCGM -t 101 -tr nnUNetTrainerV2 -m 3d_fullres --num_threads_preprocessing 1


# Result
for the final results, please follow the challenge website: https://topcow23.grand-challenge.org/evaluation/finaltest-mra-binary/leaderboard/
</br>
![image](https://github.com/orouskhani/TopCow2023/blob/main/result2.png)


# Example
![image](https://github.com/orouskhani/TopCow2023/blob/main/result.png)

