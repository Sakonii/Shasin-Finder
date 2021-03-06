# Shasin-Finder
Search for images in a folder or photo library by tags, objects present or photo description.
A computer vision approach to help finding images based on how people actually remember their photos.

## Requirements and dependencies

Dependencies installation under pip package manager

``` bash
python3 -m pip install -r requirements.txt
# If requirements.txt fails: 
# Pytorch: https://pytorch.org/get-started/locally/
# Detectron2: https://github.com/facebookresearch/detectron2/blob/master/INSTALL.md
```

## Inference

``` bash
python3 main.py --folderPath './input' --labelFile labels.csv
```

# CLI Arguments:
* '--folderPath' : Folder to search for images Default = './input'
* '--modelDetection' : Filename of weights associated with detection
* '--cfgPath' : Path to detectron model cfg file relative to 'detectron2/model_zoo'
* '--labelFile' : Path to model labels (csv file)


## Examples:

* Photo was taken in winter:

<div align="center"><img src="https://raw.githubusercontent.com/Sakonii/Shasin-Finder/main/output_examples/winter.png"></div>

* Nature, there were many animals

<div align="center"><img src="https://raw.githubusercontent.com/Sakonii/Shasin-Finder/main/output_examples/nature_animals.png"></div>

* That cat was wearing a tie

<div align="center"><img src="https://raw.githubusercontent.com/Sakonii/Shasin-Finder/main/output_examples/cat_tie.png"></div>

## Demo Video:

https://www.youtube.com/watch?v=oW-_hs5r68s&feature=youtu.be&ab_channel=UtsavMaskey
