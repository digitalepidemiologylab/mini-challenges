# pytorch-dataloader
![](https://img.shields.io/badge/difficulty-easy-brightgreen.svg)
**Skills Required :** `python`, `pytorch`

![pytorch](images/pytorch.jpeg)

We use [PyTorch](http://pytorch.org/) extensively for numerous machine learning based solutions internally.
Hence, we expect at least a basic level of familiarity with [PyTorch](http://pytorch.org/)

In this task, you are supposed to go through [this tutorial on Data Loading and Processing in PyTorch](http://pytorch.org/tutorials/beginner/data_loading_tutorial.html), and because familiar with the PyTorch [DataLoader](http://pytorch.org/docs/master/data.html#torch.utils.data.DataLoader) and [Dataset](http://pytorch.org/docs/master/data.html#torch.utils.data.Dataset) class, and implement a
custom torch `Dataset` class for the PlantVillage Dataset.

You can download the dataset from the [crowdAI PlantVillage Disease Classification Challenge](https://www.crowdai.org/challenges/plantvillage-disease-classification-challenge).
And the challenge page has more instructions about the dataset.

__NOTE__: The link to the `Test Data` is broken, so you are welcome to split the available `Training Data` into custom splits
of a configurablke

The idea is to be able to do something like this :

```python
import torch
plantvillage_dataset = YourClass(path="path-to-training-data")

plantvillage_dataloader = torch.utils.data.DataLoader(
                plantvillage_dataset,
                batch_size=128,
                shuffle=True,
                num_workers=4
                )

for images, labels in plantvillage_dataloader:
  """
    Do whatever you want the dataset
  """
  print(images.shape, labels.shape)
```

As a solution, you will have to create a publicly accessible repository, with an implementation of a custom `PlantVillageDataset` class which is derived from
the PyTorch `Dataset` class.
You also should include a section in the `README.md` on the example usage of this class with `PyTorch` `DataLoader` to load the data from the folder structure in which the images are provided.
Then you can send a pull request by including a link to your repository in the section below.

# Submitted Solutions
* `Link to your solution here`
