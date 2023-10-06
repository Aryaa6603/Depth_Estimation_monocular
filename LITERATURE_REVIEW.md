# Literature Review

## Getting Started with Monocular Depth Estimation?

*   ?

## Ideas

*   Interesting to note none of the datasets below include a lot of people. I think this might become one of the challenges of this project. [Link to issue for this idea]()

## Datasets

*   [NYU Depth Datasets V1 + V2](http://nsilberman.com/datasets/) – **V1:** Labeled data \~4GB, raw data **\~90GB**. **V2:** Labeled data \~2.8GB, raw data **\~428GB**.

    *   Indoor scenery as well as outdoor

*   [KITTI Dataset](http://www.cvlibs.net/datasets/kitti/eval_depth.php?benchmark=depth_prediction) – Annotated depth maps data \~14GB, seems entrie dataset is **\~175GB**

    *   Mainly scenery from driving

*   [DIML RGB+D Dataset](https://dimlrgbd.github.io) – Some inside and outside scenes. No faces or people.

## Relevant Links

*   [Papers w/ Code](https://paperswithcode.com/task/monocular-depth-estimation) - Monocular Depth Estimation task search.

*   [UI for non-open-source depth map from 2d image](https://3dphoto.io/uploader/) – Based on older model [Monodepth](https://github.com/mrharicot/monodepth).

## Papers

*   [BTS Paper on arXiv](https://arxiv.org/abs/1907.10326)

*   Connected Papers Graph for BTS Paper – [Interactive link](https://www.connectedpapers.com/main/4a0e8ee9eece980b54c9899977a3db0af6b8f845/From-Big-to-Small-MultiScale-Local-Planar-Guidance-for-Monocular-Depth-Estimation/graph)

## Implementations

*   [Monodepth2](https://github.com/nianticlabs/monodepth2) - **not open source**

*   [BTS-PyTorch](https://github.com/Navhkrin/Bts-PyTorch) - **Open source** implementation in pytorch of BTS which has best results on KITTI and NYU-depth-V2

*   [Vid2Depth](https://github.com/tensorflow/models/tree/master/research/vid2depth) - **Open source** Unsupervised Learning of Depth and Ego-Motion from Monocular Video Using 3D Geometric Constraints

*   [Simple Colab Demo of BTS](https://colab.research.google.com/drive/1gFee5NXeCScYuGLiHqDn8twsbUflTHJs?usp=sharing) – A straightforward to use simple app that uses the above implementation of BTS and let's users upload a photo and get a predicted depth map

