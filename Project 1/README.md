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
  - Average accuracy of this model on CelebA test set is 80.27%
