<!--
 * @Author: your name
 * @Date: 2021-06-23 14:44:02
 * @LastEditTime: 2021-06-23 14:44:03
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \undefinedc:\Users\Administrator\Desktop\Stick-figure generation with CycleGAN.md
-->
<!--
 * @Author: your name
 * @Date: 2021-06-23 14:44:02
 * @LastEditTime: 2021-06-23 14:44:02
 * @LastEditors: your name
 * @Description: In User Settings Edit
 * @FilePath: \undefinedc:\Users\Administrator\Desktop\Stick-figure generation with CycleGAN.md
-->
# Stick-figure generation with CycleGAN
This is the code for P&G task 'using GAN to generate style-transferring images'.

## Training
We train the model in a flower dataset.
```
python train.py --dataroot ./datasets/hua --name hua_cyclegan --model cycle_gan --epochs 400
```
## Testing
To prove the generalization ability of our model, the trained model can be tested on any dataset of real images.
```
python test.py --dataroot ./datasets/$YOUR DATASET --name test_cyclegan --model cycle_gan
```
where $YOUR DATASET is whatever images you want to transfer into corresponding stick-figures. In our experiment we've employed a villa dataset for testing.