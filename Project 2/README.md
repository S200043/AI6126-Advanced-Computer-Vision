Filename                                                      - Description
----------------------------------------------------------------------------------------------------
./Report.pdf                                                  - Short report
./Results/*.png                                               - Upscaled test images. [Download from here.](https://drive.google.com/file/d/1kpPvfXKkFv304XuM7WD6rjFp_bWoq01W)
./BasicSR/experiments/*/*.log                                 - Training logs
./BasicSR/options/test/SRResNet_SRGAN/test_MSRResNet_x4.yml   - BasicSR test option file
./BasicSR/options/train/SRResNet_SRGAN/train_MSRResNet_x4.yml - BasicSR training option file
./BasicSR/experiments/001_MSRResNet_x4_f64b16_DIV2K_1000k_B16G1_wandb.7000000/models/net_g_795000.pth - Model Checkpoint [Download from here.](https://drive.google.com/file/d/1roWTVWr_qf0cRzucrOthCTRrohIgHlrf)
./BasicSR/results/001_MSRResNet_x4_f64b16_DIV2K_1000k_B16G1_wandb/test_001_MSRResNet_x4_f64b16_DIV2K_1000k_B16G1_wandb_20201115_210842.log - Validation/Test log

Additional Instructions
-------------------------
To run the model checkpoint file, download the master branch of BasicSR from https://github.com/xinntao/BasicSR and extract it.
Copy the BasicSR folder in this ZIP file into the extracted folder above and overwrite all files.
Train using the commandline command: python basicsr/train.py -opt options/train/SRResNet_SRGAN/train_MSRResNet_x4.yml
Test using the commandline command: python basicsr/test.py -opt options/test/SRResNet_SRGAN/test_MSRResNet_x4.yml
The option files have already been set to use the model checkpoint file net_g_795000.pth

Mini-DIV2K Training and Validation Set - [Download from here.](https://drive.google.com/file/d/1C2iqhoPNFU5cyNAUaX3FYTMxtsAnqdDO)
Private test set with ground truth - [Download from here.](https://drive.google.com/file/d/17-a_bt0z20AuCVmIEYcHZBFaE8aFbrRx)