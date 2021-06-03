# PlaNet

The PlaNet dataset is being used to detect floating and terra firma waste debris in oceans/ports/harbors/beaches, urban and rural areas allowing the eradication of waste, helping marine life, fishermen, tourism and making the world resilient to climate change by [Recyclero](https://recyclero.com).

The dataset has been collected in a joint effort between the Recyclero and the Manipal University Jaipur. Students were able to contribute by sending their pictures of plastics, glass, paper, rubbish, metal and cardboard with our custom-built application.

## Dataset

This repository contains the dataset that we collected. The dataset spans six classes: glass, paper, cardboard, plastic, metal, and trash. Currently, the dataset consists of 2527 images,

- 501 glass
- 594 paper
- 403 cardboard
- 482 plastic
- 410 metal
- 137 trash

The pictures were taken by placing the object on a white posterboard and using sunlight and/or room lighting. The pictures have been resized down to 512 x 384, which can be changed in `dataset/constants.py` (resizing them involves going through step 1 in usage). The devices used were Apple iPhone 7 Plus, Apple iPhone 5S, and Apple iPhone SE.


## Usage: Preparing the data

If adding more data, then the new files must be enumerated properly and put into the appropriate folder in `dataset/original` and then preprocessed. Preprocessing the data involves deleting the `dataset/resized` folder and then calling `python resize.py` from `PlaNet/dataset/*`. This will take around half an hour.

### Setup

Python is currently used for some image preprocessing tasks. The Python dependencies are,

- [NumPy](http://numpy.org)
- [SciPy](http://scipy.org)

You can install these packages by running the following,

```bash
# Install using pip
pip install numpy scipy
```


## Contributing

1. Fork the repository
2. Create your feature branch using `git checkout -b my-new-feature`
3. Commit your changes using `git commit -m 'Add some feature'`
4. Push to the branch using `git push origin my-new-feature`
5. Submit a pull request


## Acknowledgments

- Stanford CS 229 (2016-2017)
- [TrashNet: Dataset of images of trash; Torch-based CNN for garbage image classification](https://github.com/garythung/trashnet)
- [AquaTrash: A dataset of Trash Images for the proper waste management and protection of Aquatic Life](https://github.com/Harsh9524/AquaTrash)
- [TACO: Trash Annotations in Context Dataset Toolkit](https://github.com/pedropro/TACO)
- [Garbage Classification - Kaggle](kaggle.com/asdasdasasdas/garbage-classification)