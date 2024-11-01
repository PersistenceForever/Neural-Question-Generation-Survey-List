# Neural Question Generation Survey
We summarize related papers and resources for neural question generation (NQG). We categorize NQG into structured NQG, unstructured NQG and hybrid NQG, as illustrated in the subsequent figure.
<img src="https://github.com/PersistenceForever/Neural-Question-Generation-Survey-List/blob/main/Taxonomy%20of%20NQG.png" with="10">

We  present a summary of the datasets widely used in NQG tasks, as shown in the Table  below.
<img src="https://github.com/PersistenceForever/Neural-Question-Generation-Survey-List/blob/main/Summary%20popular%20datasets.png" with="10">
## Table of Contents
- NQG Models
  - [Structured NQG](#structured-nqg-models)
    - [Traditional Seq2Seq Models](#traditional-seq2seq-models)
      - [RNN-based](#rnn-based)
      - [Transformer-based](#transformer-based)
    - [Graph2Seq Models](#graph2seq-models)
    - [Pre-trained Seq2Seq Models](#pre-trained-seq2seq-models)
      - [PLMs-based](#plms-based)
      - [LLMs-based](#llms-based)
  - [Unstructured NQG](#unstructured-nqg-models)
    - [Traditional Seq2Seq Models](#traditional-seq2seq-models2)
      - [RNN-based](#rnn-based2)
      - [Transformer-based](#transformer-based2)
    - [Graph-based Models](#graph-based-models)
    - [Pre-trained Seq2Seq Models](#pre-trained-seq2seq-models2)
      - [PLMs-based](#plms-based2)
      - [LLMs-based](#llms-based2)
    - [Visual2Seq Models](#visual2seq-models)
      - [CNN-based](#cnn-based)
      - [GNN-based](#gnn-based)
      - [Generative Networks-based](#generative-networks-based)
      - [PLMs-based](#plms-based3)
  - [Hybrid NQG](#hybrid-nqg-models)
    
- Benchmark Datasets
  - [Knowledge Base-based Datasets](#knowledge-base-based-datasets)
  - [Text-based Datasets](#text-based-datasets)
  - [Visual-based Datasets](#visual-based-datasets)
  
## Structured NQG Models
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
#### PLMs-based 
1. **DSM: Question Generation over Knowledge Base via Modeling Diverse Subgraphs with Meta-learner.** *Shasha Guo and Jing Zhang and Yanling Wang and Qianyi Zhang and Cuiping Li and Hong Chen*. EMNLP, 2022. [[Paper]](https://aclanthology.org/2022.emnlp-main.281.pdf) [[Code]](https://github.com/PersistenceForever/DSM)
2. **Diversifying Question Generation over Knowledge Base via External Natural Questions.** *Shasha Guo and Jing Zhang and Xirui Ke and Cuiping Li and Hong Chen*. Arxiv, 2023. [[Paper]](https://arxiv.org/pdf/2309.14362.pdf)
3. **JointGT: Graph-Text Joint Representation Learning for Text Generation from Knowledge Graphs.** *Pei Ke and Haozhe Ji and Yu Ran and Xin Cui and Liwei Wang and Linfeng Song and Xiaoyan Zhu and Minlie Huang*. ACL Findings, 2021. [[Paper]](https://arxiv.org/pdf/2106.10502.pdf) [[Code]](https://github.com/thu-coai/JointGT)
4. **LFKQG: A Controlled Generation Framework with Local Fine-tuning for Question Generation over Knowledge Bases.** *Zichu Fei and Xin Zhou and Tao Gui and Qi Zhang and Xuanjing Huang*. COLING, 2022. [[Paper]](https://aclanthology.org/2022.coling-1.572.pdf) [[Code]](https://github.com/sion-zcfei/CQG)
5. **AutoQGS: Auto-Prompt for Low-Resource Knowledge-based Question Generation from SPARQL.** *Guanming Xiong and Junwei Bao and Wen Zhao and Youzheng Wu and Xiaodong He*. CIKM, 2022. [[Paper]](https://arxiv.org/pdf/2208.12461.pdf) [[Code]](https://github.com/JimXiongGM/AutoQGS)
6. **Difficulty-controllable question generation over knowledge graphs: A counterfactual reasoning approach.** *Sheng Bi and Jianyu Liu and Zeyi Miao andQizhi Min*. Information Processing and Management, 2024. [[Paper]](https://www.sciencedirect.com/science/article/abs/pii/S0306457324000815?via%3Dihub)
#### LLMs-based
1. **Prompting Large Language Models with Chain-of-Thought for Few-Shot Knowledge Base Question Generation.** *Yuanyuan Liang and Jianing Wang and Hanlun Zhu and Lei Wang and Weining Qian and Yunshi Lan*. EMNLP, 2023. [[Paper]](https://arxiv.org/pdf/2310.08395.pdf)
2. **SGSH: Stimulate Large Language Models with Skeleton Heuristics for Knowledge Base Question Generation.** *Shasha Guo and Lizi Liao and Jing Zhang and Yanling Wang and Cuiping Li and Hong Chen*. NAACL Findings, 2024. [[Paper]](https://arxiv.org/pdf/2404.01923.pdf) [[Code]](https://github.com/PersistenceForever/SGSH)
## Unstructured NQG Models
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
8. **Multi-Hop Reasoning Question Generation and Its Application.** *Jianxing Yu and Qinliang Su and Xiaojun Quan and Jian Yin*. IEEE Trans. Knowl. Data Eng., 2023. [[Paper]](https://ieeexplore.ieee.org/document/9404866) 
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
6. **Graph augmented sequence-to-sequence model for neural question generation.** *Hui Ma and Jian Wang and Hongfei Lin and Bo Xu*. Appl. Intell., 2023. [[Paper]](https://dl.acm.org/doi/abs/10.1007/s10489-022-04260-2)
<a id="pre-trained-seq2seq-models2"></a>
### Pre-trained Seq2Seq Models
<a id="plms-based2"></a>
#### PLMs-based
1. **A Recurrent BERT-based Model for Question Generation.** *Ying-Hong Chan and Yao-Chung Fan*. MRQA@EMNLP, 2019. [[Paper]](https://aclanthology.org/D19-5821.pdf)
2. **Unified Language Model Pre-training for Natural Language Understanding and Generation.** *Dong, Li and Yang, Nan and Wang, Wenhui and Wei, Furu and Liu, Xiaodong and Wang, Yu and Gao, Jianfeng and Zhou, Ming and Hon, Hsiao-Wuen*. NeurIPS, 2019. [[Paper]](https://arxiv.org/pdf/1905.03197.pdf) [[Code]](https://github.com/microsoft/unilm)
3. **MiniLM: Deep Self-Attention Distillation for Task-Agnostic Compression of Pre-Trained Transformers.** *Wenhui Wang and Furu Wei and Li Dong and Hangbo Bao and Nan Yang and Ming Zhou*. NeurIPS, 2020. [[Paper]](https://proceedings.neurips.cc/paper/2020/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)
4. **ERNIE-GEN: An Enhanced Multi-Flow Pre-training and Fine-tuning Framework for Natural Language Generation.** *Dongling Xiao and Han Zhang and Yu-Kun Li and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang*. IJCAI, 2020. [[Paper]](https://www.ijcai.org/proceedings/2020/553) [[Code]](https://github.com/PaddlePaddle/ERNIE)
5. **Learning to generate questions by learning to recover answer-containing sentences.** *Back, Seohyun and Kedia, Akhil and Chinthakindi, Sai Chetan and Lee, Haejun and Choo, Jaegul*. ACL Findings, 2021. [[Paper]](https://aclanthology.org/2021.findings-acl.132.pdf)
6. **CoHS-CQG: Context and History Selection for Conversational Question Generation.** *Xuan Long Do and Bowei Zou and Liangming Pan and Nancy F. Chen and Shafiq R. Joty and Ai Ti Aw*. COLING, 2022. [[Paper]](https://aclanthology.org/2022.coling-1.48.pdf) [[Code]](https://github.com/dxlong2000/CoHS-CQG)
7. **Diversity Enhanced Narrative Question Generation for Storybooks.** *Hokeun Yoon and JinYeong Bak*. EMNLP, 2023. [[Paper]](https://arxiv.org/pdf/2310.16446.pdf) [[Code]](https://github.com/hkyoon95/mQG)
8. **Modeling What-to-ask and How-to-ask for Answer-unaware Conversational Question Generation.** *Xuan Long Do and Bowei Zou and Shafiq R. Joty and Anh Tran Tai and Liangming Pan and Nancy F. Chen and Ai Ti Aw*. ACL, 2023. [[Paper]](https://arxiv.org/pdf/2305.03088.pdf) [[Code]](https://github.com/dxlong2000/SG-CQG)
9. **Improving Question Generation with Multi-level Content Planning.** *Zehua Xia and Qi Gou and Bowen Yu and Haiyang Yu and Fei Huang and Yongbin Li and Cam-Tu Nguyen*. EMNLP Findings, 2023. [[Paper]](https://aclanthology.org/2023.findings-emnlp.57.pdf) [[Code]](https://github.com/zeaver/MultiFactor)
10. **TAGNet: a tiny answer-guided network for conversational question generation.** *Zekun Wang and Haichao Zhu and Ming Liu and Bing Qin*. Int. J. Mach. Learn. Cybern., 2023. [[Paper]](https://link.springer.com/article/10.1007/s13042-022-01737-x)
11. **Guiding the Growth: Difficulty-Controllable Question Generation through Step-by-Step Rewriting.** *Yi Cheng and Siyao Li and Bang Liu and Ruihui Zhao and Sujian Li and Chenghua Lin and Yefeng Zheng*. ACL/IJCNLP, 2021. [[Paper]](https://arxiv.org/pdf/2105.11698)
12. **Explainable Multi-hop Question Generation: An End-to-End Approach without Intermediate Question Labeling.** *Seonjeong Hwang and Yunsu Kim and Gary Geunbae Lee*. LREC/COLING, 2024. [[Paper]](https://arxiv.org/pdf/2404.00571) [[Code]](https://github.com/SeonjeongHwang/e2eQR)
13. **Non-Essential is NEcessary: Order-agnostic Multi-hop Question Generation.** *Kyungho Kim and Seongmin Park and Junseo Lee and Jihwa Lee*. LREC/COLING, 2024. [[Paper]](https://aclanthology.org/2024.lrec-main.1075.pdf)
14. **Agenda-Driven Question Generation: {A} Case Study in the Courtroom Domain.** *Yi Ren Fung and Anoop Kumar and Aram Galstyan and Heng Ji and Prem Natarajan*. LREC/COLING, 2024. [[Paper]](https://aclanthology.org/2024.lrec-main.49.pdf)
15. **{SGCM:} Salience-Guided Context Modeling for Question Generation.** *Chuyao Ding and Yu Hong and Jianmin Yao*. LREC/COLING, 2024. [[Paper]](https://aclanthology.org/2024.lrec-main.1285.pdf)
16. **Syntax-guided question generation using prompt learning.** *Zheheng Hou and Sheng Bi and Guilin Qi and Yuanchun Zheng and Zuomin Ren and Yun Li*. Neural Comput. Appl., 2024. [[Paper]](https://link.springer.com/article/10.1007/s00521-024-09421-7)
17. **Zero-shot Clarifying Question Generation for Conversational Search.** *Zhenduo Wang and Yuancheng Tu and Corby Rosset and Nick Craswell and Ming Wu and Qingyao Ai*. WWWW, 2023. [[Paper]](https://arxiv.org/pdf/2301.12660)
<a id="llms-based2"></a>
#### LLMs-based
1. **Towards Human-Like Educational Question Generation with Large Language Models.** *Zichao Wang and Jakob Valdez and Debshila Basu Mallick and Richard G. Baraniuk*. AIED, 2022. [[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-11644-5_13)
2. **How Teachers Can Use Large Language Models and Bloom's Taxonomy to Create Educational Quizzes.** *Sabina Elkins and Ekaterina Kochmar and Jackie C. K. Cheung and Iulian Serban*. EAAI, 2024. [[Paper]](https://arxiv.org/pdf/2401.05914)
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
<a id="plms-based3"></a>
#### PLMs-based
1. **Look before You Leap: Dual Logical Verification for Knowledge-based Visual Question Generation.** *Xumeng Liu and Wenya Guo and Ying Zhang and Xubo Liu and Yu Zhao and Shenglong Yu and Xiaojie Yuan*. LREC/COLING, 2024. [[Paper]](https://aclanthology.org/2024.lrec-main.943.pdf) [[Code]]( https://github.com/michelle19l/LV2-Net)
2. **Knowledge-Guided Cross-Topic Visual Question Generation.** *Hongfei Liu and Guohua Wang and Jiayuan Xie and Jiali Chen and Wenhao Fang and Yi Cai*. LREC/COLING, 2024. [[Paper]](https://aclanthology.org/2024.lrec-main.861.pdf)
## Hybrid NQG Models
1. **MultiQG-TI: Towards Question Generation from Multi-modal Sources.** *Zichao Wang and Richard G. Baraniuk*. ACL, 2023. [[Paper]](https://aclanthology.org/2023.bea-1.55.pdf) [[Code]](https://anonymous.4open.science/r/multimodal-QG-47F2/)
2. **ConVQG: Contrastive Visual Question Generation with Multimodal Guidance.** *Li Mi and Syrielle Montariol and Javiera Castillo Navarro and Xianjie Dai and Antoine Bosselut and Devis Tuia*. AAAI, 2024. [[Paper]](https://arxiv.org/pdf/2402.12846.pdf)
3. **A Unified Framework for Contextual and Factoid Question Generation.** *Chenhe Dong and Ying Shen and Shiyang Lin and Zhenzhou Lin and Yang Deng*. TKDE, 2024. [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10136803)
4. **Synthetic Multimodal Question Generation.** *Wu, Ian and Jayanthi, Sravan and Viswanathan, Vijay and Rosenberg, Simon and Pakazad, Sina and Wu, Tongshuang and Neubig, Graham*. Arxiv, 2024. [[Paper]](https://arxiv.org/pdf/2407.02233)
## Knowledge Base-based Datasets
1. **WebQuestions.** Introduced by *Vishwajeet Kumar and Yuncheng Hua and Ganesh Ramakrishnan and Guilin Qi and Lianli Gao and Yuan-Fang Li* in **Difficulty-controllable multi-hop question generation from knowledge graphs.** ISWC, 2019. [[Paper]](https://dl.acm.org/doi/10.1007/978-3-030-30793-6_22) [[Data]](https://github.com/liyuanfang/mhqg) [[Code]](https://github.com/liyuanfang/mhqg)
2. **PathQuestions.** Introduced by *Mantong Zhou and Minlie Huang and Xiaoyan Zhu* in **An Interpretable Reasoning Network for Multi-Relation Question Answering.** COLING, 2018. [[Paper]](https://aclanthology.org/C18-1171.pdf) [[Data]](https://github.com/zmtkeke/IRN) [[Code]](https://github.com/zmtkeke/IRN)
3. **GrailQA.** Introduced by *Yu Gu and Sue Kase and Michelle Vanni and Brian M. Sadler and Percy Liang and Xifeng Yan and Yu Su* in **Beyond I.I.D.: Three Levels of Generalization for Question Answering on Knowledge Bases.** WWW, 2021. [[Paper]](https://arxiv.org/pdf/2011.07743.pdf) [[Data]](https://dki-lab.github.io/GrailQA/) [[Code]](https://github.com/dki-lab/GrailQA)
## Text-based Datasets
1. **SQuAD.** Introduced by *Pranav Rajpurkar and Jian Zhang and Konstantin Lopyrev and Percy Liang* in **SQuAD: 100, 000+ Questions for Machine Comprehension of Text.** EMNLP, 2016. [[Paper]](https://arxiv.org/pdf/1606.05250.pdf) [[Data]](https://stanford-qa.com) [[Code]](https://stanford-qa.com)
2. **MS MARCO.** Introduced by *Tri Nguyen and Mir Rosenberg and Xia Song and Jianfeng Gao and Saurabh Tiwary and Rangan Majumder and Li Deng* in **MS MARCO: A Human Generated MAchine Reading COmprehension Dataset.** NeurIPS, 2016. [[Paper]](https://arxiv.org/pdf/1611.09268.pdf) [[Data]](https://microsoft.github.io/msmarco/) [[Code]](https://microsoft.github.io/msmarco/)
3. **NewsQA.** Introduced by *Adam Trischler and Tong Wang and Xingdi Yuan and Justin Harris and Alessandro Sordoni and Philip Bachman and Kaheer Suleman* in **NewsQA: A Machine Comprehension Dataset.** ACL, 2017. [[Paper]](https://aclanthology.org/W17-2623.pdf) [[Data]](https://www.microsoft.com/en-us/research/project/newsqa-dataset/) [[Code]](https://www.microsoft.com/en-us/research/project/newsqa-dataset/)
4. **HotpotQA.** Introduced by *Zhilin Yang and Peng Qi and Saizheng Zhang and Yoshua Bengio and William W. Cohen and Ruslan Salakhutdinov and Christopher D. Manning* in **HotpotQA: A Dataset for Diverse, Explainable Multi-hop Question Answering.** EMNLP, 2018. [[Paper]](https://arxiv.org/pdf/1809.09600.pdf)    [[Data]](https://hotpotqa.github.io/)   [[Code]](https://hotpotqa.github.io/)
5. **CoQA.** Introduced by *Siva Reddy and Danqi Chen and Christopher D. Manning* in **CoQA: A Conversational Question Answering Challenge.** TACL, 2019. [[Paper]](https://aclanthology.org/Q19-1016.pdf) [[Data]](https://stanfordnlp.github.io/coqa/) [[Code]](https://stanfordnlp.github.io/coqa/)
## Visual-based Datasets
1. **VQA.** Introduced by *Stanislaw Antol and Aishwarya Agrawal and Jiasen Lu and Margaret Mitchell and Dhruv Batra and C. Lawrence Zitnick and Devi Parikh* in **VQA: Visual Question Answering.** ICCV, 2015. [[Paper]](https://arxiv.org/pdf/1505.00468.pdf) [[Data]](https://visualqa.org/) [[Code]](https://visualqa.org/)
2. **VQG COCO.** Introduced by *Nasrin Mostafazadeh and Ishan Misra and Jacob Devlin and Margaret Mitchell and Xiaodong He and Lucy Vanderwende* in **Generating Natural Questions About an Image.** ACL, 2016. [[Paper]](https://arxiv.org/pdf/1603.06059.pdf) [[Data]](https://www.microsoft.com/en-us/download/details.aspx?id=53670) [[Code]](https://www.microsoft.com/en-us/download/details.aspx?id=53670)
3. **Visual7W** Introduced by *Yuke Zhu, Oliver Groth, Michael Bernstein, Li Fei-Fei* in **Visual7w: Grounded question answering in images.** CVPR, 2016. [[Paper]]([https://arxiv.org/pdf/1511.03416] [[Data]](https://ai.stanford.edu/~yukez/visual7w/) [[Code]](https://ai.stanford.edu/~yukez/visual7w/)
4. **FVQA** Introduced by *Peng Wang, Qi Wu, Chunhua Shen, Anton van den Hengel, Anthony Dick* in **FVQA: Fact-based Visual Question Answering.** IEEE Trans. Pattern Anal. Mach. Intell., 2018. [[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8046084) [[Data]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8046084)
