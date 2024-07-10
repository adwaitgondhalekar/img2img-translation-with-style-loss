# Unpaired Image to Image Translation using Perceptual Style Loss

Translating Images from one domain to other has been attempted with various methods, one such interesting method employed in recent times is CycleGAN. In CycleGAN two Generators are trained simultaneously, 
one for the forward mapping between the domains and one for the reverse mapping, which allows introduction of an additional loss term "Cyclic Consistency Loss" enabling both the Generators to learn the transformation effectively.
Due to the CycleGAN architecture, explicit Image pairs from both the domains are not required during training, the only requirement is presence of two sets each having images from Domain 1 and 2 respectively. CycleGAN implementation
as done in [Original Paper](https://github.com/phillipi/pix2pix) gave us good results, but our introduction of additonal loss term "Perceptual Style Loss" (inspired from [1](https://arxiv.org/abs/1508.06576) and [2](https://arxiv.org/abs/1603.08155)) 
in the overall GAN loss, gave us even better results.
Cubist and Impressionist domains of images/paintings are considered in our implementation.
 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds


## Contributors

* **Adwait Gondhalekar** - (https://github.com/adwaitgondhalekar)
* **Gunjan Payal** - (https://github.com/dxgp)

