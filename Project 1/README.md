### Filelist:  
- yongquan_chen_project1.pdf               - Report  
- Project 1/yongquan_chen_project1.ipynb   - Model code  
- Project 1/resnest50.checkpoint25.pth.tar - Checkpoint file. [Download from here.](https://drive.google.com/file/d/1eheXdPKYTk0NixkU9_RTubN4kPZmccVK)  
- Project 1/Anno/train_40_att_list.txt     - Labels from list_attr_celeba.txt partitioned according to list_eval_partition.txt  
- Project 1/Anno/val_40_att_list.txt       - Labels from list_attr_celeba.txt partitioned according to list_eval_partition.txt  
- Project 1/Anno/test_40_att_list.txt      - Labels from list_attr_celeba.txt partitioned according to list_eval_partition.txt  
- Project 1/Anno/testset.txt               - Filelist of private test set  
- Project 1/predictions.txt                - Predictions for private test set  

---

### Additional Notes:
Extract images from img_align_celeba.zip into 'Project 1/Img'  
Extract celeb subfolders into testset.zip into 'Project 1/testset'  

To train using saved checkpoint, run everything in the notebook from the top to the "Train" section.  
To test accuracy on test set, run the code in the "Test" section.  
To predict attributes for the private dataset, run the code in the "Predict" section.  

---

### Additional Files:
- Project 1/Anno/list_attr_lfwa+.txt                   - Labels for 13143 images in LFWA+ dataset from http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html  
- Project 1/Anno/lfwa+_train_40_att_list.txt           - Labels for 6263 images in LFWA+ dataset partitioned for training  
- Project 1/Anno/lfwa+_val_40_att_list.txt             - Labels for 3440 images in LFWA+ dataset partitioned for validation  
- Project 1/Anno/lfwa+_test_40_att_list.txt            - Labels for 3440 images in LFWA+ dataset partitioned for testing  
- Project 1/Anno/LFWA+/predictions.txt                 - Predictions for private test set  
- Project 1/Anno/LFWA+/resnest50.checkpoint194.pth.tar - Checkpoint file. [Download from here.](https://drive.google.com/file/d/1DHJMAzqeycPntu3COiJu0XHQs3dYkUnR/view?usp=sharing)  
  - Obtained by freezing all layers except the linear classifier layer and training on LFWA+ dataset,  
    using checkpoint 25 pretrained on CelebA.  
  - Average accuracy on CelebA test set is 80.27%  
  - Individual Accuracies:  

| Feature             | Accuracy |
|---------------------|----------|
| 5_o_Clock_Shadow    | 85.74    |
| Arched_Eyebrows     | 69.95    |
| Attractive          | 66.67    |
| Bags_Under_Eyes     | 81.36    |
| Bald                | 98.59    |
| Bangs               | 89.81    |
| Big_Lips            | 58.50    |
| Big_Nose            | 68.55    |
| Black_Hair          | 85.19    |
| Blond_Hair          | 94.91    |
| Blurry              | 95.48    |
| Brown_Hair          | 67.59    |
| Bushy_Eyebrows      | 76.31    |
| Chubby              | 91.53    |
| Double_Chin         | 91.84    |
| Eyeglasses          | 99.30    |
| Goatee              | 89.79    |
| Gray_Hair           | 97.90    |
| Heavy_Makeup        | 88.36    |
| High_Cheekbones     | 84.95    |
| Male                | 96.52    |
| Mouth_Slightly_Open | 90.27    |
| Mustache            | 93.43    |
| Narrow_Eyes         | 72.59    |
| No_Beard            | 94.49    |
| Oval_Face           | 39.21    |
| Pale_Skin           | 50.93    |
| Pointy_Nose         | 42.61    |
| Receding_Hairline   | 82.10    |
| Rosy_Cheeks         | 88.70    |
| Sideburns           | 86.10    |
| Smiling             | 92.26    |
| Straight_Hair       | 59.54    |
| Wavy_Hair           | 62.30    |
| Wearing_Earrings    | 70.75    |
| Wearing_Hat         | 98.08    |
| Wearing_Lipstick    | 93.13    |
| Wearing_Necklace    | 56.61    |
| Wearing_Necktie     | 84.54    |
| Young               | 74.21    |
