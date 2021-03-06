# Caffe常用层速查表

**备注说明**  
1. 接口对应：即表示PaddlePaddle接口与Caffe层接口基本一致，但使用者需注意参数名及参数类型  
2. PaddlePaddle实现：部分接口提供了PaddlePaddle实现的示例代码，可供用户参考  
3. 差异对比：接口存在差异，具体可查看差异对比文档  

| 序号 | Caffe层                                                      | PaddlePaddle接口                                             | 备注                                                         |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1    | [AbsVal](http://caffe.berkeleyvision.org/tutorial/layers/absval.html) | [paddle.fluid.layers.abs](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-182-abs) | 接口对应                                                     |
| 2    | [Accuracy](http://caffe.berkeleyvision.org/tutorial/layers/accuracy.html) | [paddle.fluid.layers.accuracy](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-253-accuracy) | [差异对比](Accuracy.md) |
| 3    | [ArgMax](http://caffe.berkeleyvision.org/tutorial/layers/argmax.html) | [paddle.fluid.layers.argmax](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-204-argmax) | [差异对比](ArgMax.md) |
| 4    | [BatchNorm](http://caffe.berkeleyvision.org/tutorial/layers/batchnorm.html) | [paddle.fluid.layers.batch_norm](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-36-batch_norm) | [差异对比](BatchNorm.md) |
| 5    | [BNLL](http://caffe.berkeleyvision.org/tutorial/layers/bnll.html) | [paddle.fluid.layers.softplus](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-194-softplus) | 接口对应                                                     |
| 6    | [Concat](http://caffe.berkeleyvision.org/tutorial/layers/concat.html) | [paddle.fluid.layers.concat](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-209-concat) | 接口对应                                                     |
| 7    | [Convolution](http://caffe.berkeleyvision.org/tutorial/layers/convolution.html) | [paddle.fluid.layers.conv2d](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-45-conv2d) | [差异对比](Convolution.md) |
| 8    | [Crop](http://caffe.berkeleyvision.org/tutorial/layers/crop.html) | [paddle.fluid.layers.crop](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-51-crop) | [差异对比](Crop.md) |
| 9    | [Deconvolution](http://caffe.berkeleyvision.org/tutorial/layers/deconvolution.html) | [paddle.fluid.layers.conv2d_transpose](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-46-conv2d_transpose) | [差异对比](Deconvolution.md) |
| 10   | [Dropout](http://caffe.berkeleyvision.org/tutorial/layers/dropout.html) | [paddle.fluid.layers.dropout](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-56-dropout) | [差异对比](Dropout.md) |
| 11   | [Eltwise](http://caffe.berkeleyvision.org/tutorial/layers/eltwise.html) | -                                                            | [PaddlePaddle实现](Eltwise.md) |
| 12   | [ELU](http://caffe.berkeleyvision.org/tutorial/layers/elu.html) | [paddle.layers.fluid.elu](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-68-elu) | 接口对应                                                     |
| 13   | [EuclideanLoss](http://caffe.berkeleyvision.org/tutorial/layers/euclideanloss.html) | [paddle.fluid.layers.square_error_cost](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-167-square_error_cost) | [差异对比](EuclideanLoss.md) |
| 14   | [Exp](http://caffe.berkeleyvision.org/tutorial/layers/exp.html) | [paddle.fluid.layers.exp](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-186-exp) | [差异对比](Exp.md) |
| 15   | [Flatten](http://caffe.berkeleyvision.org/tutorial/layers/flatten.html) | [paddle.fluid.layer.reshape](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-72-reshape) | [差异对比](Flatten.md) |
| 16   | [InnerProduct](http://caffe.berkeleyvision.org/tutorial/layers/innerproduct.html) | [paddle.fluid.layers.fc](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-71-fc) | [差异对比](InnerProduct.md) |
| 17   | [Input](http://caffe.berkeleyvision.org/tutorial/layers/input.html) | [paddle.fluid.layers.data](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-20-data) | [差异对比](Input.md) |
| 18   | [Log](http://caffe.berkeleyvision.org/tutorial/layers/log.html) | [paddle.fluid.layers.log](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-93-log) | [差异对比](Log.md) |
| 19   | [LRN](http://caffe.berkeleyvision.org/tutorial/layers/lrn.html) | [paddle.fluid.layers.lrn](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-99-lrn) | [差异对比](LRN.md) |
| 20   | [Pooling](http://caffe.berkeleyvision.org/tutorial/layers/pooling.html) | [paddle.fluid.layers.pool2d](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-115-pool2d) | [差异对比](Pooling.md) |
| 21   | [Power](http://caffe.berkeleyvision.org/tutorial/layers/power.html) | [paddle.fluid.layers.pow](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-117-pow) | [差异对比](Power.md) |
| 22   | [PReLU](http://caffe.berkeleyvision.org/tutorial/layers/prelu.html) | [paddle.layers.fluid.prelu](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-118-prelu) | 接口对应                                                     |
| 23   | [Reduction](http://caffe.berkeleyvision.org/tutorial/layers/reduction.html) | -                                                            | [PaddlePaddle实现](Reduction.md) |
| 24   | [ReLU](http://caffe.berkeleyvision.org/tutorial/layers/relu.html) | -                                                            | [PaddlePaddle实现](ReLU.md) |
| 25   | [Reshape](http://caffe.berkeleyvision.org/tutorial/layers/reshape.html) | [paddle.fluid.layers.reshape](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-130-reshape) | [差异对比](Reshape.md) |
| 26   | [Scale](http://caffe.berkeleyvision.org/tutorial/layers/scale.html) | [paddle.fluid.layers.scale](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-137-scale) | [差异对比](Scale.md) |
| 27   | [SigmoidCrossEntropyLoss](http://caffe.berkeleyvision.org/tutorial/layers/sigmoidcrossentropyloss.html) | [paddle.fluid.layers.sigmoid_cross_entropy_with_logits](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-158-sigmoid_cross_entropy_with_logits) | [差异对比](SigmoidCrossEntropyLoss.md) |
| 28   | [Sigmoid](http://caffe.berkeleyvision.org/tutorial/layers/sigmoid.html) | [paddle.fluid.layers.sigmoid](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-192-sigmoid) | 接口对应                                                     |
| 29   | [Slice](http://caffe.berkeleyvision.org/tutorial/layers/slice.html) | [paddle.fluid.layers.slice](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-160-slice) | [差异对比](Slice.md) |
| 30   | [SoftmaxWithLoss](http://caffe.berkeleyvision.org/tutorial/layers/softmaxwithloss.html) | [paddle.fluid.layers.softmax_with_cross_entropy](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-164-softmax_with_cross_entropy) | [差异对比](SofmaxWithLoss.md) |
| 31   | [Softmax](http://caffe.berkeleyvision.org/tutorial/layers/softmax.html) | [paddle.fluid.layers.softmax](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-163-softmax) | [差异对比](Sofmax.md) |
| 32   | [TanH](http://caffe.berkeleyvision.org/tutorial/layers/tanh.html) | [paddle.fluid.layers.tanh](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-199-tanh) | 接口对应                                                     |
| 33   | [Tile](http://caffe.berkeleyvision.org/tutorial/layers/tile.html) | [paddle.fluid.layers.expand](http://paddlepaddle.org/documentation/docs/zh/1.3/api_cn/layers_cn.html#permalink-70-expand) | [差异对比](Tile.md) |
