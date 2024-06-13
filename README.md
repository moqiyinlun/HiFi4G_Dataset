# HiFi4G Dataset
The dataset of the paper "HiFi4G: High-Fidelity Human Performance Rendering via Compact Gaussian Splatting".

## HiFi4G: High-Fidelity Human Performance Rendering via Compact Gaussian Splatting

**[Yuheng Jiang](https://nowheretrix.github.io/), [Zhehao Shen](https://github.com/moqiyinlun), [Penghao Wang](https://authoritywang.github.io/), Zhuo Su, [Yu Hong](https://github.com/xyi1023), [Yingliang Zhang](https://cn.linkedin.com/in/yingliangzhang), [Jingyi Yu](http://www.yu-jingyi.com/), [Lan Xu](http://xu-lan.com/).** 

*CVPR 2024*

[[Project Page]](https://nowheretrix.github.io/HiFi4G/) [[Paper Link]](https://arxiv.org/abs/2312.03461)

![dataset_description](./imgs/gallery.png)

### Description

We have currently uploaded 6 sample cases of data with different people and diverse motions. Meanwhile, 3 single-frame data have been uploaded as examples, which you can access without signing the license agreement.

To run algorithms on single-frame data, you need to move the calibration files. For `image_white` under instant-ngp format, rename the frame folder to `images` and move `transforms.json` to the same directory as `images`. For `image_white_undistortion` in colmap format, rename the frame folder to `images` and move the `sparse/0` folder to the same directory as `images`.

The overall file structure is as follows:
```
├── image_white
│    ├── %d                - The frame number, starts from 0.
│    │   └──%d.png         - Masked RGB images for each view. view number starts from 0.
│    └── transforms.json   - Camera extrinsics and intrinsics in NGP format.
│
├── image_white_undistortion
│    ├── %d                - The frame number, starts from 0.
│    │   └──%d.png         - Undistorted maksed RGB images for each view. view number starts from 0.
│    └── colmap/sparse/0   - Camera extrinsics and intrinsics in Gaussian Splatting format.
```
### Download our dataset

The dataset is available on Onedrive and requires permission to access it. Please carefully read, fill in the [license form](./license.pdf), and send it to Yuheng Jiang (jiangyh2@shanghaitech.edu.cn) and cc Lan Xu(xulan1@shanghaitech.edu.cn) to request access.

By requesting access to the content, you acknowledge that you have read this agreement, understand it, and agree to be bound by its terms and conditions. This agreement constitutes a legal and binding agreement between you and the provider of the protected system or content. The Virtual Reality and Visual Computing Center is the only owner of all intellectual property rights, including copyright, of HiFi4G Dataset, and VRVC reserves the right to terminate your access to the dataset at any time.

Notes:

Once the license agreement is signed, we will give access to the data.

### Citation

If you use this dataset for your research, please cite our paper:

```
@InProceedings{Jiang_2024_CVPR,
 author = {Jiang, Yuheng and Shen, Zhehao and Wang, Penghao and Su, Zhuo and Hong, Yu and Zhang, Yingliang and Yu, Jingyi and Xu, Lan}, 
 title = {HiFi4G: High-Fidelity Human Performance Rendering via Compact Gaussian Splatting}, 
 booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)}, 
 month = {June}, 
 year = {2024}, 
 pages = {19734-19745} 
 }
```



