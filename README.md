# Overview

This repo contains code for the "TensorFlow for poets 2" series of codelabs.

# Usage

1. Clone the repository using:
```
git clone https://github.com/therohitramesh/flower-recog.git
```
2. Run the script specifying an image.
```
python -m scripts.label_image [--image IMAGE] \ [--graph GRAPH]
```

## For example to run the script for a daisy flower:

![daisy](https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/img/3021186b83bc90c2.png)

Run this is in the terminal: `python -m scripts.label_image     --graph=tf_files/retrained_graph.pb
     --image=tf_files/flower_photos/roses/2414954629_3708a1a04d.jpg`

# How can you use it to train other categories?

In theory, all you need to do is run the tool, specifying a particular set of sub-folders. Each sub-folder is named after one of your categories and contains only images from that category.

If you complete this step and pass the root folder of the subdirectories as the argument for the --image_dir parameter, the script should train the images that you've provided, just like it did for the flowers.

The classification script uses the folder names as label names, and the images inside each folder should be pictures that correspond to that label.



# Note
The `scripts` directory contains helpers for the codelab. Some of these come from the main TensorFlow repository, and are included here so you can use them without also downloading the main TensorFlow repo (they are not part of the TensorFlow `pip` installation).
