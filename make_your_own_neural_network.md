# Python神经网络编程(Make Your Own Neural Network)
## 第1章 神经网络如何工作
### 1.1 尺有所短, 寸有所长
### 1.2 一台简单的预测机
### 1.3 分类器与预测器并无太大差别
### 1.4 训练简单的分类器
- 使用朴素的调整方法会出现一个问题, 即改进后的模型只与最后一次训练样本最匹配, "有效地"忽略了是所有以前的训练样本. 解决这个问题的一种好方法试试随时用学习率, 调节改进速率, 这样单一的训练样本就不能主导整个学习过程.
- 来自真实世界的训练样本可能充满噪声或包含错误. 适度更新有助于限制这些错误样本的影响
### 1.5 有时候一个分类器不足以求解问题
- 如果数据本身不是由单一线性过程支配, 那么一个简单的线性分类器不能对数据进行划分. 例如, 由逻辑 XOR运算符支配的数据说明了这一点
- 但是解决方案很容易, 你只需要使用多个线性分类器来划分由单一直线无法分离的数据.
### 1.6 神经元——大自然的计算机器
### 1.7 在神经网络中追踪信号
### 1.8 凭心而论, 矩阵乘法大有用途
- 通过神经网络向前馈送信号所需的大量运算可以表示为矩阵乘法
### 1.9 使用矩阵乘法的三层神经网络示例
### 1.10 学习来自多个节点的权重
### 1.11 多个输出节点反向传播误差
### 1.12 反向传播误差到更多层中
- 按照链接权重的比例来分割输出层的误差, 然后在每个内部节点处重组这些误差
### 1.13 使用矩阵乘法进行反向传播误差
- 反向传播误差可以表示为矩阵乘法
- 向前馈送信号和反向传播误差都可以使用矩阵计算而变得高效
### 1.14 我们实际上如何更新权重
- __梯度下降法__ 是求解函数最小值的一种很好的办法
- 神经网络的误差是内部链接权重的函授
- 改进神经网络, 意味着通过改变权重减少这种误差
- 通过误差函数的梯度下降, 采取小步长, 迭代地改进权重. 所迈出的每一步的方向都是在当前位置向下斜率最大的方向, 这就是所谓的梯度下降
### 1.15 权重更新成功范例
### 1.16 准备数据
- 饱和: 大信号(有时候是由大权重带来的)导致了应用在信号上的激活函数的斜率变得非常平缓. 这降低了神经网络学习到更好权重的能力
- 零值信号或零值权重. 使神经网络丧失学习更好权重的能力
- 输出应该在激活函数能够生成的值的范围内. 逻辑 S函数是不可能生成小于等于 0或大于等于 1的值. 将训练目标值上设置在有效的范围之外, 将会驱使产生越来越大的权重, 导致网络饱和. 一个合适的范围为 0.01 ~ 0.99
## 第2章 使用Python进行DIY
### 2.1 Python
### 2.2 交互式Python = IPython
### 2.3 优雅地开始使用 Python
### 2.4 使用Python制作神经网络
### 2.5 手写数字的数据集MNIST
## 第3章 趣味盎然
### 3.1 自己的手写数字
### 3.2 神经网络大脑的内部
### 3.3 创建新的训练数据: 旋转图像
### 3.4 结语
