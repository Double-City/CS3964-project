# README

## 传统风格迁移

- 传统风格迁移文件夹包含两部分代码，分别是做纹理缝合和做纹理迁移的代码。

- 若是运行纹理缝合代码，请在命令行内输入

  ```python
  python3 main.py --synthesis -i <path of texture_img> -b <block_size> -o <overlap_size> -t <tolerance>
  ```

- 若是运行纹理迁移代码，请在命令行内融入

  ```python
  python3 main.py --transfer -i1 <path of style_img> -i2 <path of content_img> -b <block_size> -o <overlap_size> -t <tolerance> -a <alpha>
  ```

- 除了上面两个命令行可调整的参数，其他可调参数可输入

  ```python
  python3 main.py -h
  ```

- 除了代码，文件夹里还包含 img_style 风格图片文件夹和 img_content 内容图片文件夹可供使用，并且有我们已经跑出来的结果，放在 output 文件夹里。

## 现代风格迁移

- 现代风格迁移文件夹包含两部分代码，分别是做固定风格的普通迁移 tran.ipynb 和固定风格的快速迁移 batch_tran.ipynb。

- 在 tran.ipynb 中，在第二个代码块可导入风格图像和内容图像，第七个代码块可更改训练轮数。在 batch_tran.ipynb 中，第二个代码块可导入风格图像，第七个代码块可导入内容图像集，第十一个代码块展示了可调参数。

- 除了代码，文件夹里还包含 img_style 风格图片文件夹和 img_content、coco数据集 内容图片文件夹可供使用，以及噪声图像 noise.jpg、white.jpg 并且有我们已经跑出来的结果和 loss 图像，放在 output、loss 文件夹里。

## 个人贡献

- 在合作项目中负责实验环境的搭建，基于现代深度神经网络的算法的解释以及部分报告的攥写，并且负责部分参数的调试以及神经网络的训练过程
