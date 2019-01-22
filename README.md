# AlgorithmContests
### 背景：
一张图片上有两个字符，并有重叠的情况，字符色度差别一般在20-40个色度之间。同一个字符的渲染色度都是一个固定值范围内波动，对重叠部分的色度基本用 alpaha_blending 混合，会增加一定的底板噪声和平滑。
### 要求：
将这两个字符和底板进行分离。语义分割处理后结果以灰度图作为输入：<br>  
底板：0<br>  
字符非重叠部分：60和120<br>  
字符重叠部分：180<br>  
字符包括大小写英文和数字（没有汉字了）。<br>  
### 评分：
part1:按格式上传测试集分割结果，占总分30%。<br>  
part2：源代码和完整的算法文档压缩包，根据真实场景和可推广性打分，70%<br>  
### 注意事项：
1.统计像素、穷举等不能用。<br>  
2.语言限制Python，框架推荐tenseorFlow或pytorch。<br>  
3.算法文档包括论文引用和具体实现细节。<br>  
### 数据集说明：
数据集包含两个文件夹 img 以及 label，分别为生成的训练图片以及相应的标记图片，标记图片为灰度图，0 代表底板，60 和 120 代表相应字符不重叠区域，180 代表字符重叠部分所在区域。
### 日程：
3 月初会发布结果提交页面，包含测试集压缩包，分割结果和代码文档压缩包提交入口，结果提交后不可再更改。
### 参考文献：
1.Semantic Image Segmentation with Deep Convolutional Nets and Fully Connected CRFs<br>  
2.DeepLab: Semantic Image Segmentation with Deep Convolutional Nets, Atrous Convolution, and Fully Connected CRFs<br>  
3.Rethinking Atrous Convolution for Semantic Image Segmentation<br>  
4.Fully Convolutional Networks for Semantic Segmentation<br>  
5.Segmentation of Brain MR Images Through a Hidden Markov Random Field Model and the Expectation-Maximization Algorithm<br>  
6.“GrabCut” —— Interactive Foreground Extraction using Iterated Graph Cuts<br>  
7.Efficient Inference in Fully Connected CRFs with Gaussian Edge Potentials<br>  
