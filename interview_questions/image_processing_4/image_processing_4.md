# 31
# opencv读取图像存储的顺序为什么是BGR，而不是RGB？
从历史原因，当时主流的摄像头制造商和软件供应商提供的摄像头采集的图像的通道排列顺序为BGR
另外对图片来说，位图BMP是最简单的，也是Windows显示图片的基本格式，在Windows下，任何格式的图片文件，包括视频播放，都需要先转化为位图才能显示出来，而位图BMP的格式就是BGR，其他格式的图片文件是在位图格式基础上采用不同的压缩算法生成的。


# 如何计算存储灰度图所需的比特数b？

b = M * N * k
其中
b：数字图像所需的比特数
MN：数字图像的长宽
k：由灰度级算出，公式：L = 2^k
例子：
一张图片大小为1920x1080，256个灰度级的图像，需要多少个byte来存储
由256个灰度级---->256 = 2 ^k----->k==8
所以b = 1920x1080x8

