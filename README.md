# tricks
## Samples
样本合成工具<br>
data augmentagion: flip, Random Crop, blur, dropout & ensemble, clip, linefitting, Aspect Ratio, Random Rotation, Pixel Jitter, Random Mirror, 贴背景,shift,zoom, motion blur, Erosion and dilation, down sampling, gaussion noise, elastic distortion, <br>
提取人工特征作为输入，比如：ldp,hog<br>

## loss
triplet loss<br>
smooth L1 loss-outlier<br>
overfitting-L1/L2 regularization<br>

## training
boosting<br>
learning rate一开始大后来小，合适的lr训练轮数多点，学习率很小的时候，训练轮数可以很少<br>
batchnorm<br>
dropout<br>
residual<br>
deep<br>
3*3 kernel<br>
finetune<br>
relu<br>
[online hard sample mining](https://arxiv.org/abs/1604.03540)-keep positive=1, normal negative=1.5, hard negative=1.5<br>
归一化，减均值除方差，可以是训练集的统计值，也可以是单个样本的统计值<br>
global average pooling<br>
U-Net，multi-scale<br>
lstm慢，可以代替方案，将视频上一帧的网络的输出作为下一帧网络的输入<br>
backbone<br>
[deep mutual learning](http://openaccess.thecvf.com/content_cvpr_2018/CameraReady/0304.pdf)<br>

## algorithm
multi-task: object detection<br>
md-lstm/spatio-temporal-lstm<br>
attention<br>
1d conv<br>
net-vlad<br>
moe-mixture of experts<br>
ensemble<br>
gating: video classification<br>
radical-based: chinese character recognition<br>
stack stages on the top of network: openpose<br>
deconv后，和原图尺寸不同可以使用autocrop (Richer Convolutional Features for Edge Detection)
soft-nms
deformable convolution
cascade

## tools
tensorflow：tensorpack、slim<br>

## 加速
    tensorRT加速3-4倍
    轻量级网络：mobilenet、shufflenet
### 手机端
    ncnn(tencent), cpu
    mace(xiaomi), cpu & gpu

## 特征定长
lstm/gru<br>
vlad<br>
padding/cut<br>
roi pooling<br>
attention<br>

## optimization
SGD<br>
adam<br>
AdaDelta<br>
Nesterov accelerated gradient(NAG)<br>

## filler
constant<br>
gaussian<br>
positive_unitball<br>
uniform<br>
xavier - relu, 2010<br>
msra - relu, hekaiming2015<br>
bilinear - deconv<br>
