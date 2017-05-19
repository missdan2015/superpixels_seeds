# superpixels_seeds
超像素分割方法，采用论文 SEEDS: Superpixels Extracted via Energy-Driven Sampling 提出的方法，对于物体的边界具有较好的保留，如下图所示。可以辅助目标检测中制作Banchmark。


本工程在其基础上，获得的图像labels和contours，然后分别实现区域种子填充，Windows下编译环境为：
OpenCV
CMake
Visual Studio
工程demo包括：

SuperSeedsTest: SEEDS 提供的用例，可获取超像素分割labels和contours
SeedFillTest : 基于labels种子填充子块
BoundaryFillTest : 基于contours种子填充子块

备注：无需配置cmake也行，自己手动添加文件头文件和源文件
