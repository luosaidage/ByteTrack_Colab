# ByteTrack

## Demo Links
| Google Colab Demo | Huggingface Demo |                  YouTube Tutorial                   | Original Paper: ByteTrack |
|:-----------------:|:----------------:|:---------------------------------------------------:|:-------------------------:|
|[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1bDilg4cmXFa8HCKHbsZ_p16p0vrhLyu0?usp=sharing)|[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/akhaliq/bytetrack)|[![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/QCG8QMhga9k)|[arXiv 2110.06864](https://arxiv.org/abs/2110.06864) |
* Integrated to [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio).


## Abstract
Multi-object tracking (MOT) aims at estimating bounding boxes and identities of objects in videos. Most methods obtain identities by associating detection boxes whose scores are higher than a threshold. The objects with low detection scores, e.g. occluded objects, are simply thrown away, which brings non-negligible true object missing and fragmented trajectories. To solve this problem, we present a simple, effective and generic association method, tracking by associating every detection box instead of only the high score ones. For the low score detection boxes, we utilize their similarities with tracklets to recover true objects and filter out the background detections. When applied to 9 different state-of-the-art trackers, our method achieves consistent improvement on IDF1 scores ranging from 1 to 10 points. To put forwards the state-of-the-art performance of MOT, we design a simple and strong tracker, named ByteTrack. For the first time, we achieve 80.3 MOTA, 77.3 IDF1 and 63.1 HOTA on the test set of MOT17 with 30 FPS running speed on a single V100 GPU.
<p align="center"><img src="assets/teasing.png" width="400"/></p>

## News
* (2022.07) Our paper is accepted by ECCV 2022!
* (2022.06) A [nice re-implementation](https://github.com/PaddlePaddle/PaddleDetection/tree/develop/configs/mot/bytetrack) by Baidu [PaddleDetection](https://github.com/PaddlePaddle/PaddleDetection)!
