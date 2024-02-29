# 基础概念补充
##1、马尔科夫链
  扩散概率模型（简称为“扩散模型”）是一个参数化的马尔可夫链。
  马尔科夫链为状态空间中经过从一个状态到另一个状态的转换的随机过程，该过程要求具备“无记忆性 ”，即下一状态的概率分布只能由当前状态决定，在时间序列中它前面的事件均与之无关。这种特定类型的“无记忆性 ”称作马尔可夫性质。
  https://zhuanlan.zhihu.com/p/448575579
##2、自回归和自编码模型
  应用总述https://zhuanlan.zhihu.com/p/625714067
  AR模型通常用于生成式任务，在长文本的生成能力很强，比如自然语言生成（NLG）领域的任务：摘要、翻译或抽象问答。
  AE模型通常用于内容理解任务，比如自然语言理解（NLU）中的分类任务：情感分析、提取式问答。
  AR原理详解https://zhuanlan.zhihu.com/p/435442095
  AE原理详解https://zhuanlan.zhihu.com/p/133207206
##3、GAP
  训练过程中存在的差距或间隙，这个间隙可能表示两者之间在性能、效果或其他方面的差异或不足之处。
  例如在多模态训练过程中：深度学习模型输出的embedding往往会聚集在一个狭小的锥形空间内，不同随机初始化产生的embedding会分布在不同的锥形区域，导致不同模态之间存在明显的差距。这种现象可能受到深度学习模型本身结构、激活函数以及网络层数等因素的影响
#扩散模型学习记录
##1、DDPM（概率去噪扩散模型）
  前向加噪和反向去噪，讲解视频：https://www.bilibili.com/video/BV1tz4y1h7q1/?spm_id_from=333.999.0.0&vd_source=12b452817cc2c0420d8edd85f6438257
  论文：《Denoising Diffusion Probabilistic Models》
  code：https://github.com/hojonathanho/diffusion
