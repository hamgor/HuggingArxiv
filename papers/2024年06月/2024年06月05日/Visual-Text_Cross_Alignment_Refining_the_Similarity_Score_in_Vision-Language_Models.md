# 视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度

发布时间：2024年06月05日

`RAG

这篇论文主要关注的是视觉-语言模型的应用，特别是在零-shot学习场景下的性能提升。论文提出了一种新的方法——加权视觉-文本交叉对齐（WCA），这种方法通过局部视觉提示技术和预训练的视觉-语言模型（如CLIP）来提高图像与文本描述的对齐精度。这种方法的提出和实证分析表明，它能够显著提升零-shot性能，并且在多个数据集上进行了验证。因此，这篇论文更符合RAG分类，即研究如何通过改进模型和方法来提升相关任务的性能。` `计算机视觉`

> Visual-Text Cross Alignment: Refining the Similarity Score in Vision-Language Models

# 摘要

> 近期研究表明，利用预训练的视觉-语言模型（如CLIP），将查询图像与大型语言模型生成的多个精细文本描述对齐，能大幅提升零-shot性能。但本文实证指出，这些精细描述更擅长与图像的局部区域而非整体对齐，并通过理论分析证实了这一点。为此，我们提出了一种新颖的加权视觉-文本交叉对齐（WCA）方法。该方法首先采用局部视觉提示技术，精准定位查询图像中的关键视觉区域，随后通过预训练VLM构建的相似度矩阵，实现这些区域与文本描述的精准匹配。我们进一步设计了一个基于加权相似度的评分函数，以评估图像与各类别的对齐质量。实验结果显示，WCA方法在多个数据集上显著提升了零-shot性能，其效果甚至可与少-shot学习方法媲美。

> It has recently been discovered that using a pre-trained vision-language model (VLM), e.g., CLIP, to align a whole query image with several finer text descriptions generated by a large language model can significantly enhance zero-shot performance. However, in this paper, we empirically find that the finer descriptions tend to align more effectively with local areas of the query image rather than the whole image, and then we theoretically validate this finding. Thus, we present a method called weighted visual-text cross alignment (WCA). This method begins with a localized visual prompting technique, designed to identify local visual areas within the query image. The local visual areas are then cross-aligned with the finer descriptions by creating a similarity matrix using the pre-trained VLM. To determine how well a query image aligns with each category, we develop a score function based on the weighted similarities in this matrix. Extensive experiments demonstrate that our method significantly improves zero-shot performance across various datasets, achieving results that are even comparable to few-shot learning methods.

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x1.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x2.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x3.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x4.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x5.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x6.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x7.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x9.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x10.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x11.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x12.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x13.png)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/eurosat_overview_small.jpg)

![视觉与文本的精准对齐：提升视觉-语言模型中的相似度评分精度](../../../paper_images/2406.02915/x14.png)

[Arxiv](https://arxiv.org/abs/2406.02915)