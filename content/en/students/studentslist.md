+++
draft = false
+++

### Lab Members 

#### Director 
Yue Dong, assistant professor of computer science and engineering 

#### PhD Students 
- Yu Fu, since Fall 2023
- Zehao Wang (co-advise with [Dr. Heng Yin](https://www.cs.ucr.edu/~heng/)), since Fall 2023
- [Erfan Shayegani](https://erfanshayegani.github.io/) (co-advise with [Dr. Nael B. Abu-Ghazaleh](https://www.cs.ucr.edu/~nael/)), since Summer 2023


#### MSc Students 
- Niyathi Allu 
- Priyanshu Sharma
- Lohith Kumar Bhambore


### Research 

The primary research objective of the UCR NLP lab is to create trustworthy, controllable, and safe natural language processing tools that can understand, reason, and produce human-like texts. The trustworthiness encompasses multiple facets, including producing useful but harmless content (AI safety), being detectable for responsible use (AI detection), being fair towards different social groups (AI fairness), and being factual with respect to context and world knowledge (hallucination reduction). To meet this objective, we are committed to interdisciplinary research, incorporating methods and tools from natural language processing, machine learning, reinforcement learning, explainable AI, cybersecurity, optimization, and computer vision. Following are some selected research areas we focus on.


#### Trustworthy NLP - Hallucination Reduction 

The main trustworthy aspect that our research lab is interested in pertains to the study of natural language understanding and generation. We aim to gain insight into why models hallucinate and how facts are processed in deep neural networks. Additionally, our research has been focused on hallucination reduction techniques for conditional text generation, particularly in the areas of text summarization and dialogue.

Previously Proposed methods include (i) using weakly supervised learning for fact error correction, as cited in [1], question-answering systems [2], and knowledge graphs [3]; and (ii) innovative learning [4] and detection approaches [5] for factual generation. These approaches have led to significant improvements in hallucination reduction, as measured by faithfulness metrics and human evaluations.


**Related paper:**
- Factual Error Correction for Abstractive Summarization Models.  Cao, M., Dong, Y., Wu, J., & Cheung, J.   EMNLP 2020
- Multi-Fact Correction in Abstractive Text Summarization. Dong, Y., Wang, S., Gan, Z., Cheng, Y., Cheung, J. , & Liu, J.  EMNLP2020
- Faithful to the Document or to the World? Mitigating Hallucinations via Entity-Linked Knowledge in Abstractive Summarization. Dong, Y.,  Wieting, J., Verga, P. Findings of EMNLP 2022.
- Learning with Rejection for Abstractive Text Summarization.Cao, M., Dong, Y., He, J., & Cheung, J.  EMNLP 2022
- Hallucinated but Factual! Inspecting the Factuality of Hallucinations in Abstractive Summarization. Cao, M., Dong, Y., & Cheung, J.  ACL 2022.


### AI Safety

#### Large Language Models (LLMs) Vulnerability 

Large language models are demonstrating cutting-edge performance across a diverse range of application domains. However, the widespread implementation of these models (e.g., GPT-4) into autonomous systems is hindered by their vulnerability to adversarial attacks in the field of machine learning. Adversaries can introduce subtle alterations into input data, causing the model to make erroneous classifications or harmful generations. This vulnerability can lead to hazardous consequences, exemplified by instances where a stop sign might be misconstrued as a speed limit sign, or where generative models instruct individuals on creating explosives or influencing elections.

One emerging trend involves integrating various types of data—such as text, images, and audio—into large language models. However, the inclusion of publicly available vision encoders like CLIP (Contrastive Language–Image Pre-training) into these complex systems introduces an underexplored vulnerability: it allows adversaries to exploit the system even with black-box access. As detailed in our paper (http://arxiv.org/abs/2307.14539), this vulnerability presents significant security risks for a wide range of applications that depend on multi-modal models. 


Additionally, humans have the ability to identify and fix problematic text triggers. However, our plug-and-play adversarial attack embeds these prompts within seemingly harmless images. This makes the attack difficult to patch and highly adaptable across platforms. As a result, these concealed prompts can guide language models to act maliciously in systems that handle both text and images.  #LLMs #AIsafety #NLProc


**Related paper:**
- Plug and Pray: Exploiting off-the-shelf components of Multi-Modal Models, Shayegani, E., Dong, Y., Abu-Ghazaleh, N., arXiv preprint arXiv:2307.14539


####  AI Generation Detection (Security and Privacy)
The increasing prevalence of new iterations of generative AI models, which learn to predict the next tokens in a sequence, has raised concerns about the potential malicious use of human-like outputs. One solution to such concerns is to add watermarks to texts generated by AI, enabling AI generation detection. By aiming to develop robust methods for AI generation detection, we can mitigate risks and better understand how to integrate AI into society responsibly.


To mitigate potential risks associated with language models (LMs), recent AI detection research proposes incorporating watermarks into machine-generated text through random vocabulary restrictions and utilizing this information for detection. In this paper, we show that watermarking algorithms designed for LMs cannot be seamlessly applied to conditional text generation (CTG) tasks without a notable decline in downstream task performance. To address this issue, we introduce a simple yet effective semantic-aware watermarking algorithm that considers the characteristics of conditional text generation with the input context. Compared to the baseline watermarks, our proposed watermark yields significant improvements in both automatic and human evaluations across various text generation models, including BART and Flan-T5, for CTG tasks such as summarization and data-to-text generation. Meanwhile, it maintains detection ability with higher z-scores but lower AUC scores, suggesting the presence of a detection paradox that poses additional challenges for watermarking CTG. 


**Related paper:**
- Watermarking Conditional Text Generation for AI Detection: Unveiling Challenges and a Semantic-Aware Watermark Remedy, Fu, Y., Xiong, D., Dong, Y., arXiv preprint arXiv:2307.13808




