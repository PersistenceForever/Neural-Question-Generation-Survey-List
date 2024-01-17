# Neural-Question-Generation-Survey-List
We summarize related research papers and resources for neural question generation (Neural QG). We categorize Neural QG into structured QG and unstructured QG, as illustrated in the subsequent figure.
<img src="https://github.com/PersistenceForever/Neural-Question-Generation-Survey-List/blob/main/Taxonomy%20of%20neural%20QG.png" with="10">
## Table of Contents
- Neural QG
  - [Structured QG](#structured-qg)
    - [Traditional Seq2Seq Models](#traditional-seq2seq-models)
      - [RNN-based](#rnn-based)
      - [Transformer-based](#transformer-based)
    - [Graph2Seq Models](#graph2seq-models)
    - [Pre-trained Seq2Seq Models](#pre-trained-seq2seq-models)
      - [Encoder-Decoder Transformer-based](#encoder-decoder-transformer-based)
      - [Decoder-only Transformer-based](#decoder-only-transformer-based)
  - [Unstructured QG](#unstructured-qg)
    - [Traditional Seq2Seq Models](#traditional-seq2seq-models2)
      - [RNN-based](#rnn-based2)
      - [Transformer-based](#transformer-based2)
    - [Graph-based Models](#graph-based-models)
    - [Pre-trained Seq2Seq Models](#pre-trained-seq2seq-models2)
    - [Visual2Seq Models](#visual2seq-models)
      - [CNN-based](#cnn-based)
      - [GNN-based](#gnn-based)
      - [Generative Networks-based](#generative-networks-based)
## Structured QG
### Traditional Seq2Seq Models
#### RNN-based
1. **Generating natural language question-answer pairs from a knowledge graph using a RNN based question generation model.** *Sathish Reddy Indurthiand Dinesh Raghu and Mitesh M Khapra and Sachindra Joshi*. EACL, 2017. [[Paper]](https://aclanthology.org/E17-1036.pdf)
2. **Zero-shot question generation from knowledge graphs for unseen predicates and entity types.** *Hady Elsahar and Christophe Gravier and Frederique Laforest*. NAACL, 2018. [[Paper]](https://aclanthology.org/N18-1020.pdf) [[Code]](https://github.com/hadyelsahar/Zeroshot-QuestionGeneration)
3. **Knowledge-enriched, Type-constrained and Grammar-guided Question Generation over Knowledge Bases.** *Sheng Bi and Xiya Cheng and YuanFang Li and Yongzhen Wang and Guilin Qi*. COLING, 2020. [[Paper]](https://arxiv.org/pdf/2010.03157.pdf) [[Code]](https://github.com/bisheng/MultiHopQG)
#### Transformer-based
1. **Generating Questions for Knowledge Bases via Incorporating Diversified Contexts and Answer-Aware Loss.** *Cao Liu and Kang Liu and Shizhu He and Zaiqing Nie and Jun Zhao*. EMNLP, 2019. [[Paper]](https://arxiv.org/pdf/1910.13108.pdf)
2. **Difficulty-controllable multi-hop question generation from knowledge graphs.** *Vishwajeet Kumar and Yuncheng Hua and Ganesh Ramakrishnan and Guilin Qi and Lianli Gao and Yuan-Fang Li*. ISWC, 2019. [[Paper]](https://link.springer.com/chapter/10.1007/978-3-030-30793-6_22) [[Code]](https://github.com/liyuanfang/mhqg)
### Graph2Seq Models
1. **KGPT: Knowledge-Grounded Pre-Training for Data-to-Text Generation.** *Chen, Wenhu and Su, Yu and Yan, Xifeng and Wang, William Yang*. EMNLP, 2020. [[Paper]](https://aclanthology.org/2020.emnlp-main.697.pdf) [[Code]](https://github.com/wenhuchen/KGPT)
2. **Meta-CQG: A Meta-Learning Framework for Complex Question Generation over Knowledge Bases.** *Kun Zhang and Yunqi Qiu and Yuanzhuo Wang and Long Bai and Wei Li and Xuhui Jiang and Huawei Shen and Xueqi Cheng*. COLING, 2022. [[Paper]](https://aclanthology.org/2022.coling-1.533.pdf)
3. **Toward Subgraph-Guided Knowledge Graph Question Generation With Graph Neural Networks.** *Yu Chen and Lingfei Wu and Mohammed J. Zaki*. TNNLS, 2023. [[Paper]](https://arxiv.org/pdf/2004.06015.pdf) [[Code]](https://github.com/hugochan/Graph2Seq-for-KGQG)
### Pre-trained Seq2Seq Models
#### Encoder-Decoder Transformer-based 
1. **JointGT: Graph-Text Joint Representation Learning for Text Generation from Knowledge Graphs.** *Pei Ke and Haozhe Ji and Yu Ran and Xin Cui and Liwei Wang and Linfeng Song and Xiaoyan Zhu and Minlie Huang*. ACL Findings, 2021. [[Paper]](https://arxiv.org/pdf/2106.10502.pdf) [[Code]](https://github.com/thu-coai/JointGT)
2. **DSM: Question Generation over Knowledge Base via Modeling Diverse Subgraphs with Meta-learner.** *Shasha Guo and Jing Zhang and Yanling Wang and Qianyi Zhang and Cuiping Li and Hong Chen*. EMNLP, 2022. [[Paper]](https://aclanthology.org/2022.emnlp-main.281.pdf) [[Code]](https://github.com/PersistenceForever/DSM)
3. **LFKQG: A Controlled Generation Framework with Local Fine-tuning for Question Generation over Knowledge Bases.** *Zichu Fei and Xin Zhou and Tao Gui and Qi Zhang and Xuanjing Huang*. COLING, 2022. [[Paper]](https://aclanthology.org/2022.coling-1.572.pdf) [[Code]](https://github.com/sion-zcfei/CQG)
4. **AutoQGS: Auto-Prompt for Low-Resource Knowledge-based Question Generation from SPARQL.** *Guanming Xiong and Junwei Bao and Wen Zhao and Youzheng Wu and Xiaodong He*. CIKM, 2022. [[Paper]](https://arxiv.org/pdf/2208.12461.pdf) [[Code]](https://github.com/JimXiongGM/AutoQGS)
5. **Diversifying Question Generation over Knowledge Base via External Natural Questions.** *Shasha Guo and Jing Zhang and Xirui Ke and Cuiping Li and Hong Chen*. Arxiv, 2023. [[Paper]](https://arxiv.org/pdf/2309.14362.pdf)
#### Decoder-only Transformer-based
1. **Prompting Large Language Models with Chain-of-Thought for Few-Shot Knowledge Base Question Generation.** *Yuanyuan Liang and Jianing Wang and Hanlun Zhu and Lei Wang and Weining Qian and Yunshi Lan*. EMNLP, 2023. [[Paper]](https://arxiv.org/pdf/2310.08395.pdf)
## Unstructured QG
<a id="traditional-seq2seq-models2"></a>
### Traditional Seq2Seq Models
<a id="rnn-based2"></a>
#### RNN-based
1. **Learning to Ask: Neural Question Generation for Reading Comprehension.** *Du, Xinya and Shao, Junru and Cardie, Claire*. ACL, 2017. [[Paper]](https://aclanthology.org/P17-1123.pdf) [[Code]](https://github.com/xinyadu/nqg)
2. **Answer-focused and position-aware neural question generation.** *Sun, Xingwu and Liu, Jing and Lyu, Yajuan and He, Wei and Ma, Yanjun and Wang, Shi*. EMNLP, 2018. [[Paper]](https://aclanthology.org/D18-1427.pdf)
3. **Harvesting Paragraph-level Question-Answer Pairs from Wikipedia.** *Du, Xinya and Cardie, Claire*. ACL, 2018. [[Paper]](https://aclanthology.org/P18-1177.pdf) [[Code]](https://github.com/xinyadu/HarvestingQA)
4. **Neural Models for Key Phrase Extraction and Question Generation.** *Sandeep Subramanian and Tong Wang and Xingdi Yuan and Saizheng Zhang and Adam Trischler and Yoshua Bengio*. ACL, 2018. [[Paper]](https://aclanthology.org/W18-2609.pdf)
5. **Improving Question Generation With to the Point Context.** *Jingjing Li and Yifan Gao and Lidong Bing and Irwin King and Michael R. Lyu*. EMNLP, 2019. [[Paper]](https://aclanthology.org/D19-1317.pdf)
6. **Improving Neural Question Generation Using Answer Separation.** *Yanghoon Kim and Hwanhee Lee and Joongbo Shin and Kyomin Jung*. AAAI, 2019. [[Paper]](https://arxiv.org/pdf/1809.02393.pdf)
7. **Capturing Greater Context for Question Generation.** *Luu Anh Tuan and Darsh J. Shah and Regina Barzilay*. AAAI, 2020. [[Paper]](https://arxiv.org/pdf/1910.10274.pdf)
<a id="transformer-based2"></a>
#### Transformer-based
1. **Cross-Lingual Training for Automatic Question Generation.** *Vishwajeet Kumar and Nitish Joshi and Arijit Mukherjee and Ganesh Ramakrishnan and Preethi Jyothi*. ACL, 2019. [[Paper]](https://aclanthology.org/P19-1481.pdf) [[Code]](https://github.com/vishwajeet93/clqg)
2. **Neural question generation with answer pivot.** *Wang, Bingning and Wang, Xiaochuan and Tao, Ting and Zhang, Qi and Xu, Jingfang*. AAAI, 2020. [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/6449)
3. **Learning to ask more: Semi-autoregressive sequential question generation under dual-graph interaction.** *Zi Chai and Xiaojun Wan*. ACL, 2020. [[Paper]](https://aclanthology.org/2020.acl-main.21.pdf) [[Code]](https://github.com/ChaiZ-pku?tab=repositories)
### Graph-based Models
1. **Reinforcement Learning Based Graph-to-Sequence Model for Natural Question Generation.** *Chen, Yu and Wu, Lingfei and Zaki, Mohammed J.Zaki*. ICLR, 2020. [[Paper]](https://arxiv.org/pdf/1908.04942.pdf) [[Code]](https://github.com/hugochan/RL-based-Graph2Seq-for-NQG)
2. **Semantic Graphs for Generating Deep Questions.** *Liangming Pan and Yuxi Xie and Yansong Feng and Tat-Seng Chua and Min-Yen Kan*. ACL, 2020. [[Paper]](https://arxiv.org/pdf/2004.12704.pdf) [[Code]](https://github.com/WING-NUS/SG-Deep-Question-Generation)
3. **Multi-hop Question Generation with Graph Convolutional Network.** *Dan Su and Yan Xu and Wenliang Dai and Ziwei Ji and Tiezheng Yu and Pascale Fung*. EMNLP Findings, 2020. [[Paper]](https://aclanthology.org/2020.findings-emnlp.416.pdf) [[Code]](https://github.com/HLTCHKUST/MulQG)
4. **Iterative GNN-based decoder for question generation.** *Fei, Zichu and Zhang, Qi and Zhou, Yaqian*. EMNLP, 2021. [[Paper]](https://aclanthology.org/2021.emnlp-main.201.pdf) [[Code]](https://github.com/sion-zcfei/IGND)
5. **CQG: A Simple and Effective Controlled Generation Framework for Multi-hop Question Generation.** *Zichu Fei and Qi Zhang and Tao Gui and Di Liang and Sirui Wang and Wei Wu and Xuanjing Huang*. ACL, 2022. [[Paper]](https://aclanthology.org/2022.acl-long.475.pdf) [[Code]](https://github.com/sion-zcfei/CQG)
6. **Modeling What-to-ask and How-to-ask for Answer-unaware Conversational Question Generation.** *Xuan Long Do and Bowei Zou and Shafiq R. Joty and Anh Tran Tai and Liangming Pan and Nancy F. Chen and Ai Ti Aw*. ACL, 2023. [[Paper]](https://arxiv.org/pdf/2305.03088.pdf) [[Code]](https://github.com/dxlong2000/SG-CQG)
<a id="pre-trained-seq2seq-models2"></a>
### Pre-trained Seq2Seq Models
1. **A Recurrent BERT-based Model for Question Generation.** *Ying-Hong Chan and Yao-Chung Fan*. MRQA@EMNLP, 2019. [[Paper]](https://aclanthology.org/D19-5821.pdf)
2. **Unified Language Model Pre-training for Natural Language Understanding and Generation.** *Dong, Li and Yang, Nan and Wang, Wenhui and Wei, Furu and Liu, Xiaodong and Wang, Yu and Gao, Jianfeng and Zhou, Ming and Hon, Hsiao-Wuen*. NeurIPS, 2019. [[Paper]](https://arxiv.org/pdf/1905.03197.pdf) [[Code]](https://github.com/microsoft/unilm)
3. **MiniLM: Deep Self-Attention Distillation for Task-Agnostic Compression of Pre-Trained Transformers.** *Wenhui Wang and Furu Wei and Li Dong and Hangbo Bao and Nan Yang and Ming Zhou*. NeurIPS, 2020. [[Paper]](https://proceedings.neurips.cc/paper/2020/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)
4. **ERNIE-GEN: An Enhanced Multi-Flow Pre-training and Fine-tuning Framework for Natural Language Generation.** *Dongling Xiao and Han Zhang and Yu-Kun Li and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang*. IJCAI, 2020. [[Paper]](https://www.ijcai.org/proceedings/2020/553) [[Code]](https://github.com/PaddlePaddle/ERNIE)
5. **Learning to generate questions by learning to recover answer-containing sentences.** *Back, Seohyun and Kedia, Akhil and Chinthakindi, Sai Chetan and Lee, Haejun and Choo, Jaegul*. ACL Findings, 2021. [[Paper]](https://aclanthology.org/2021.findings-acl.132.pdf)
6. **Improving Question Generation with Multi-level Content Planning.** *Zehua Xia and Qi Gou and Bowen Yu and Haiyang Yu and Fei Huang and Yongbin Li and Cam-Tu Nguyen*. EMNLP Findings, 2023. [[Paper]](https://aclanthology.org/2023.findings-emnlp.57.pdf) [[Code]](https://github.com/zeaver/MultiFactor)
### Visual2Seq Models
#### CNN-based
1. **Visual question generation as dual task of visual question answering.** *Li, Yikang and Duan, Nan and Zhou, Bolei and Chu, Xiao and Ouyang, Wanli and Wang, Xiaogang and Zhou, Ming*. CVPR, 2018. [[Paper]](https://ieeexplore.ieee.org/document/8578738)
2. **iVQA: Inverse Visual Question Answering.** *Feng Liu and Tao Xiang and Timothy M. Hospedales and Wankou Yang and Changyin Sun*. CVPR, 2018. [[Paper]](https://arxiv.org/pdf/1710.03370.pdf)
3. **Difficulty-Controllable Visual Question Generation.** *Feng Chen and Jiayuan Xie and Yi Cai and Tao Wang and Qing Li*. APWeb-WAIM, 2021. [[Paper]](https://link.springer.com/chapter/10.1007/978-3-030-85896-4_26)
4. **Deconfounded Visual Question Generation with Causal Inference.** *Jiali Chen and Zhenjun Guo and Jiayuan Xie and Yi Cai and Qing Li*. ACM MM, 2023. [[Paper]](https://dl.acm.org/doi/10.1145/3581783.3612536) [[Code]](https://github.com/Gary-code/KECVQG)
#### GNN-based
1. **Radial graph convolutional network for visual question generation.** *Xu, Xing and Wang, Tan and Yang, Yang and Hanjalic, Alan and Shen, Heng Tao*. TNNLS, 2020. [[Paper]](https://ieeexplore.ieee.org/document/9079208) [[Code]](https://github.com/Wangt-CN/VQG-GCN)
2. **Multiple objects-aware visual question generation.** *Xie, Jiayuan and Cai, Yi and Huang, Qingbao and Wang, Tao*. ACM MM, 2021. [[Paper]](https://dl.acm.org/doi/abs/10.1145/3474085.3476969)
3. **Knowledge-Based Visual Question Generation.** *Jiayuan Xie and Wenhao Fang and Yi Cai and Qingbao Huang and Qing Li*. IEEE Trans. Circuits Syst. Video Technol., 2022. [[Paper]](https://ieeexplore.ieee.org/document/9826805)
4. **Visual Question Generation Under Multi-granularity Cross-Modal Interaction.** *Zi Chai and Xiaojun Wan and Soyeon Caren Han and Josiah Poon*. MMM, 2023. [[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-27077-2_20)
#### Generative Networks-based
1. **Information Maximizing Visual Question Generation.** *Ranjay Krishna and Michael S. Bernstein and Li Fei-Fei*. CVPR, 2019. [[Paper]](https://arxiv.org/pdf/1903.11207.pdf)
2. **C3VQG: category consistent cyclic visual question generation.** *Shagun Uppal and Anish Madan and Sarthak Bhagat and Yi Yu and Rajiv Ratn Shah*. ACM MM Asia, 2020. [[Paper]](https://dl.acm.org/doi/10.1145/3444685.3446302) [[Code]](https://github.com/sarthak268/C3VQG-official)
