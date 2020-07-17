# ODMS
Object Depth via Motion and Segmentation Dataset

Contact: Brent Griffin (griffb at umich dot edu)

## Publication
Please cite our [paper](https://arxiv.org/abs/2007.05676 "ECCV Paper") if you find it useful for your research.
```
@inproceedings{GrCoECCV20,
  author = {Griffin, Brent A. and Corso, Jason J.},
  booktitle={The European Conference on Computer Vision (ECCV)},
  title = {Learning Object Depth from Camera Motion and Video Object Segmentation},
  year = {2020}
}
```

## Quick Introduction

__ECCV 2020 Supplementary Video:__ https://youtu.be/c90Fg_whjpI

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/c90Fg_whjpI/0.jpg)](https://youtu.be/c90Fg_whjpI)

## Using ODMS

__Run__ ``./demo/demo_datagen.py`` <br />
Generates random data for ODMS training. Example configurations are provided in the ``./config/`` folder. Provides the option to save a static dataset as well. <br />
[native Python, has scipy dependency]

__Run__ ``./demo/demo_dataset_eval.py`` <br />
Evaluates a depth estimation model on the ODMS validation and test sets. An example evaluation is provided for the VOS-DE baseline. Results are saved in the ``./results/`` folder. <br />
[native Python, VOS-DE baseline has skimage dependency]

## Benchmark

| Method | Robot | Driving | Normal | Perturb | All |
| --------------- | --------------- | --------------- | --------------- | --------------- | --------------- |
| [ODN-lr](https://arxiv.org/abs/2007.05676 "ECCV Paper") | 13.1 | 31.7 | 8.6 | 17.9 | 17.8 |
| [VOS-DE](https://arxiv.org/abs/1903.08336) | 32.6 | 36.0 | 7.9 | 33.6 | 27.5 |

Is your technique missing although it's published and the code is public? Let us know and we'll add it.

## Use

This code is available for non-commercial research purposes only.