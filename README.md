# MRBrainS18 MISPL challenge winning code

Winning submission to the Grand Challenge on MR Brain Segmentation at MICCAI 2018.

* [Check the challenge results](http://mrbrains18.isi.uu.nl/results/eight-label-segmentation-results/)
* [Download pretrained weights](https://drive.google.com/file/d/1MU6XEU5OE4Z2UgjCbxPoSdES0i2JZvUr/view?usp=sharing)
* Check our paper [3D Patchwise U-Net with Transition Layers for MR Brain Segmentation](https://www.springer.com/gp/book/9783030117221)


## Usage

Create a python environment able to run the packages Numpy, TensorFlow and SimpleITK. Then you can execute the commands according to the required task as follows.

### Training

```bash
bash run.sh <run number> train <GPU number> <checkpoint number>
```

```bash
bash run.sh 1 train 0 0
```

### Testing

```bash
bash run.sh <run number> test <GPU number> <checkpoint number>
```

```bash
bash run.sh 1 test 0 0
```

### Summaries

```bash
bash run.sh <run number> summaries <GPU number>
```

```bash
bash run.sh 1 summaries 0
```

### Update global summary

```bash
bash get_summaries.sh
```

### Check the summaries file

```bash
cat summary.txt
```
