# Unpaired Image to Image Translation using Perceptual Style Loss

Translating Images from one domain to other has been attempted with various methods, one such interesting method employed in recent times is CycleGAN. In CycleGAN two Generators are trained simultaneously, 
one for the forward mapping between the domains and one for the reverse mapping, which allows introduction of an additional loss term "Cyclic Consistency Loss" enabling both the Generators to learn the transformation effectively.
Due to the CycleGAN architecture, explicit Image pairs from both the domains are not required during training, the only requirement is presence of two sets each having images from Domain 1 and 2 respectively. CycleGAN implementation
as done in [Original Paper](https://github.com/phillipi/pix2pix) gave us good results, but our introduction of additonal loss term "Perceptual Style Loss" ( inspired from [1](https://arxiv.org/abs/1508.06576) and [2](https://arxiv.org/abs/1603.08155) ) 
in the overall GAN loss, gave us even better results.
Cubist and Impressionist domains of images/paintings are considered in our implementation.
 

## Getting Started

### Prerequisites
* Python 3.10+
* Dependencies as given in [requirements](./requirements.txt)
* Dataset containing images from both domains
* Directory structure to be used for the dataset inside project directory
```
    ├── data                  
        ├── trainA       #to contain images from domain A                    
        ├── trainB       #to contain images from domain B
```

## Results
* #### Images labeled as "Original X" correspond to Cubist Images.
* #### Images labeled as "Original Y" correspond to Impressionist Images.
* #### Images labeled as "Transformed X" correspond to Cubist Images translated to Impressionist Images.
* #### Images labeled as "Transformed Y" correspond to Impressionist Images translated to Cubist Images.
* #### Images labeled as "Reconstructed X" correspond to Cubist Images that went through Cyclic translation <br> (Cubist->Impressionist->Cubist).
* #### Images labeled as "Reconstructed Y" correspond to Impressionist Images that went through Cyclic translation <br> (Impressionist->Cubist->Impressionist).

![result 1](https://github.com/adwaitgondhalekar/img2img-translation-with-style-loss/blob/main/results/output_1.jpg)

![result 2](https://github.com/adwaitgondhalekar/img2img-translation-with-style-loss/blob/main/results/output_2.jpg)

![result 3](https://github.com/adwaitgondhalekar/img2img-translation-with-style-loss/blob/main/results/output_3.jpg)

![result 4](https://github.com/adwaitgondhalekar/img2img-translation-with-style-loss/blob/main/results/output_4.jpg)



## Contributors

* **Adwait Gondhalekar** - (https://github.com/adwaitgondhalekar)
* **Gunjan Payal** - (https://github.com/dxgp)

