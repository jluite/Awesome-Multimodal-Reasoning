<h1 align="center">Awesome Multimodal Reasoning</h1>

<p align="center">
    <img src="https://awesome.re/badge.svg" href="https://github.com/atfortes/Awesome-Multimodal-Reasoning"/>
    <img src="https://img.shields.io/badge/License-MIT-green.svg" href="https://opensource.org/licenses/MIT"/>
    <img src="https://img.shields.io/badge/PRs-Welcome-red"/>
    <img src="https://img.shields.io/github/last-commit/atfortes/Awesome-Multimodal-Reasoning?color=green"/>
</p>

<p align="center">
    <b> Collection of papers and resources on how to unlock reasoning abilities under multimodal settings.</b>
</p>

<p align="center">
    <img src="https://github.com/cvlab-columbia/viper/blob/main/teaser.gif" width="100%" style="align:center;"/>
</p>

<p align="right">
    <i>Animation from <a href="https://viper.cs.columbia.edu/">ViperGPT (Surís et al.)</a></i>
</p>

<p align="center">
    Consider how difficult it would be to study from a book that lacks any figures, diagrams or tables. We enhance our learning ability when we combine different data modalities, such as vision, language, and audio <a href="https://arxiv.org/abs/2302.00923">[1]</a>. Recently, large language models (LLMs) have achieved remarkable results in complex reasoning tasks by generating intermediate steps before deducing the answer via chain-of-thought (CoT) reasoning <a href="https://arxiv.org/abs/2201.11903">[2]</a> <a href="https://github.com/atfortes/LLM-Reasoning-Papers">[3]</a>. However, most of the research on CoT reasoning only involves the language modality and not others. We present a collection of papers and resources on how to unlock these abilities under multimodal settings.
</p>



## Contents



 - [Technique](#technique)
    - [End-to-end Models](#e2e)
    - [Prompting & In-context Learning](#prompt)
    - [Compositional & Symbolic Approach](#symbolic)
 - [Benchmark](#benchmark)
 - [Other Useful Resources](#other-useful-resources)
 - [Other Awesome Lists](#other-awesome-lists)
 - [Contributing](#contributing)


 
## Technique
 
<h3 id="e2e">End-to-end Models</h3>
 
 

1. **Learning to Reason: End-to-End Module Networks for Visual Question Answering.** `ICCV 2017`

    *Ronghang Hu, Jacob Andreas, Marcus Rohrbach, Trevor Darrell, Kate Saenko.* [[Paper](https://arxiv.org/abs/1704.05526)], 2017.4

1. **Flamingo: a Visual Language Model for Few-Shot Learning.** `NeurIPS 2022`

    *Jean-Baptiste Alayrac, Jeff Donahue, Pauline Luc, Antoine Miech, Iain Barr, Yana Hasson, Karel Lenc, Arthur Mensch, Katie Millican, Malcolm Reynolds, Roman Ring, Eliza Rutherford, Serkan Cabi, Tengda Han, Zhitao Gong, Sina Samangooei, Marianne Monteiro, Jacob Menick, Sebastian Borgeaud, Andrew Brock, Aida Nematzadeh, Sahand Sharifzadeh, Mikolaj Binkowski, Ricardo Barreira, Oriol Vinyals, Andrew Zisserman, Karen Simonyan.* [[Blog](https://www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-model)] [[Paper](https://arxiv.org/abs/2204.14198)], 2022.4

1. **BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models.** `Preprint`

    *Junnan Li, Dongxu Li, Silvio Savarese, Steven Hoi.* [[Paper](https://arxiv.org/abs/2301.12597)] [[Code](https://github.com/salesforce/LAVIS/tree/main/projects/blip2)], 2023.1

1. **Language Is Not All You Need: Aligning Perception with Language Models.** `Preprint`

    *Shaohan Huang, Li Dong, Wenhui Wang, Yaru Hao, Saksham Singhal, Shuming Ma, Tengchao Lv, Lei Cui, Owais Khan Mohammed, Barun Patra, Qiang Liu, Kriti Aggarwal, Zewen Chi, Johan Bjorck, Vishrav Chaudhary, Subhojit Som, Xia Song, Furu Wei.* [[Paper](https://arxiv.org/abs/2302.14045)], 2023.2

1. **Prismer: A Vision-Language Model with An Ensemble of Experts.** `Preprint`

    *Shikun Liu, Linxi Fan, Edward Johns, Zhiding Yu, Chaowei Xiao, Anima Anandkumar.* [[Project](https://shikun.io/projects/prismer)] [[Paper](https://arxiv.org/abs/2303.02506)] [[Code](https://github.com/NVlabs/prismer)] [[Demo](https://huggingface.co/spaces/lorenmt/prismer)], 2023.3

1. **PaLM-E: An Embodied Multimodal Language Model.** `Preprint`

    *Danny Driess, Fei Xia, Mehdi S. M. Sajjadi, Corey Lynch, Aakanksha Chowdhery, Brian Ichter, Ayzaan Wahid, Jonathan Tompson, Quan Vuong, Tianhe Yu, Wenlong Huang, Yevgen Chebotar, Pierre Sermanet, Daniel Duckworth, Sergey Levine, Vincent Vanhoucke, Karol Hausman, Marc Toussaint, Klaus Greff, Andy Zeng, Igor Mordatch, Pete Florence.* [[Project](https://palm-e.github.io/)] [[Paper](https://arxiv.org/abs/2303.03378)], 2023.3

1. **GPT-4 Technical Report.** `Preprint`

    *OpenAI.* [[Blog](https://openai.com/research/gpt-4)] [[Paper](https://arxiv.org/abs/2303.08774)], 2023.3

1. **Visual Instruction Tuning.** `Preprint`

    *Haotian Liu, Chunyuan Li, Qingyang Wu, Yong Jae Lee.* [[Project](https://llava-vl.github.io/)] [[Paper](https://arxiv.org/abs/2304.08485)] [[Code](https://github.com/haotian-liu/LLaVA)] [[Demo](https://llava.hliu.cc/)], 2023.4

1. **MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models.** `Preprint`

    *Deyao Zhu, Jun Chen, Xiaoqian Shen, Xiang Li, Mohamed Elhoseiny.* [[Project](https://minigpt-4.github.io/)] [[Paper](https://arxiv.org/abs/2304.10592)] [[Code](https://github.com/Vision-CAIR/MiniGPT-4)], 2023.4

1. **Otter: A Multi-Modal Model with In-Context Instruction Tuning** `Preprint`

    *Bo Li, Yuanhan Zhang, Liangyu Chen, Jinghao Wang, Jingkang Yang, Ziwei Liu.* [[Paper](https://arxiv.org/abs/2305.03726)] [[Code](https://github.com/Luodian/Otter)], 2023.5 

1. **VisionLLM: Large Language Model is also an Open-Ended Decoder for Vision-Centric Tasks.** `Preprint`

    *VisionLLM: Large Language Model is also an Open-Ended Decoder for Vision-Centric Tasks.* [[Paper](https://arxiv.org/abs/2305.11175)] [[Code](https://github.com/OpenGVLab/VisionLLM)] [[Demo](https://github.com/OpenGVLab/InternGPT)], 2023.5

1. **Kosmos-2: Grounding Multimodal Large Language Models to the World** `Preprint`

    *Zhiliang Peng, Wenhui Wang, Li Dong, Yaru Hao, Shaohan Huang, Shuming Ma, Furu Wei.* [[Paper](https://arxiv.org/abs/2306.14824)], 2023.6

1. **BuboGPT: Enabling Visual Grounding in Multi-Modal LLMs.** `Preprint`

    *Yang Zhao, Zhijie Lin, Daquan Zhou, Zilong Huang, Jiashi Feng, Bingyi Kang.* [[Paper](https://arxiv.org/abs/2307.08581)] [[Code](https://bubo-gpt.github.io/)], 2023.7

1. **Augmenting CLIP with Improved Visio-Linguistic Reasoning.** `Preprint`

    *Samyadeep Basu, Maziar Sanjabi, Daniela Massiceti, Shell Xu Hu, Soheil Feizi.* [[Paper](https://arxiv.org/abs/2307.09233)], 2023.7

1. **Med-Flamingo: a Multimodal Medical Few-shot Learner.** `Preprint`

    *Michael Moor, Qian Huang, Shirley Wu, Michihiro Yasunaga, Cyril Zakka, Yash Dalmia, Eduardo Pontes Reis, Pranav Rajpurkar, Jure Leskovec.* [[Paper](https://arxiv.org/abs/2307.15189)] [[Code](https://github.com/snap-stanford/med-flamingo)], 2023.7

1. **Qwen-VL: A Frontier Large Vision-Language Model with Versatile Abilities.** `Preprint`

    *Jinze Bai, Shuai Bai, Shusheng Yang, Shijie Wang, Sinan Tan, Peng Wang, Junyang Lin, Chang Zhou, Jingren Zhou.* [[Paper](https://arxiv.org/abs/2308.12966)] [[Code](https://github.com/QwenLM/Qwen-VL)], 2023.8

1. **Kosmos-2.5: A Multimodal Literate Model.** `Preprint`

    *Tengchao Lv, Yupan Huang, Jingye Chen, Lei Cui, Shuming Ma, Yaoyao Chang, Shaohan Huang, Wenhui Wang, Li Dong, Weiyao Luo, Shaoxiang Wu, Guoxin Wang, Cha Zhang, Furu Wei.* [[Paper](https://arxiv.org/abs/2309.11419)], 2023.9

1. **Improved Baselines with Visual Instruction Tuning.** `Preprint`

   *Haotian Liu, Chunyuan Li, Yuheng Li, Yong Jae Lee.* [[Project](https://llava-vl.github.io/)] [[Paper](https://arxiv.org/abs/2310.03744)] [[Code](https://github.com/haotian-liu/LLaVA)], 2023.10

1. **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model.** `Preprint`

   *Jiahui Gao, Renjie Pi, Jipeng Zhang, Jiacheng Ye, Wanjun Zhong, Yufei Wang, Lanqing Hong, Jianhua Han, Hang Xu, Zhenguo Li, Lingpeng Kong.* [[Paper](https://arxiv.org/abs/2312.11370)], 2023.12

1. **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model.** `Preprint`

   *Jiahui Gao, Renjie Pi, Jipeng Zhang, Jiacheng Ye, Wanjun Zhong, Yufei Wang, Lanqing Hong, Jianhua Han, Hang Xu, Zhenguo Li, Lingpeng Kong.* [[Paper](https://arxiv.org/abs/2312.11370)], 2023.12

1. **Gemini: A Family of Highly Capable Multimodal Models.** `Preprint`

   *Gemini Team, Google.* [[Paper](https://arxiv.org/abs/2312.11805)], 2023.12

1. **Gemini: A Family of Highly Capable Multimodal Models.** `Preprint`

   *Gemini Team, Google.* [[Paper](https://arxiv.org/abs/2312.11805)], 2023.12

1. **Gemini in Reasoning: Unveiling Commonsense in Multimodal Large Language Models.** `Preprint`

   *Yuqing Wang, Yun Zhao.* [[Paper](https://arxiv.org/abs/2312.17661)], 2023.12



<h3 id="prompt">Prompting & In-context Learning</h3>



1. **Multimodal Few-Shot Learning with Frozen Language Models.** `NeurIPS 2021`

    *Multimodal Few-Shot Learning with Frozen Language Models.* [[Paper](https://arxiv.org/abs/2106.13884)], 2021.6

1. **Socratic Models: Composing Zero-Shot Multimodal Reasoning with Language.** `ICLR 2023`

    *Andy Zeng, Maria Attarian, Brian Ichter, Krzysztof Choromanski, Adrian Wong, Stefan Welker, Federico Tombari, Aveek Purohit, Michael Ryoo, Vikas Sindhwani, Johnny Lee, Vincent Vanhoucke, Pete Florence.* [[Project](https://socraticmodels.github.io/)] [[Paper](https://arxiv.org/abs/2204.00598)] [[Code](https://github.com/google-research/google-research/tree/master/socraticmodels)], 2022.4

1. **Multimodal Chain-of-Thought Reasoning in Language Models.** `Preprint`

    *Zhuosheng Zhang, Aston Zhang, Mu Li, Hai Zhao, George Karypis, Alex Smola.* [[Paper](https://arxiv.org/abs/2302.00923)] [[Code](https://github.com/amazon-science/mm-cot)], 2023.2

1. **Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models.** `Preprint`

    *Chenfei Wu, Shengming Yin, Weizhen Qi, Xiaodong Wang, Zecheng Tang, Nan Duan.* [[Paper](https://arxiv.org/abs/2303.04671)] [[Code](https://github.com/microsoft/visual-chatgpt)], 2023.3

1. **MM-REACT: Prompting ChatGPT for Multimodal Reasoning and Action.** `Preprint`

    *Zhengyuan Yang, Linjie Li, Jianfeng Wang, Kevin Lin, Ehsan Azarnasab, Faisal Ahmed, Zicheng Liu, Ce Liu, Michael Zeng, Lijuan Wang.* [[Project](https://multimodal-react.github.io/)] [[Paper](https://arxiv.org/abs/2303.11381)] [[Code](https://github.com/microsoft/MM-REACT)] [[Demo](https://huggingface.co/spaces/microsoft-cognitive-service/mm-react)], 2023.3

1. **Visual Chain of Thought: Bridging Logical Gaps with Multimodal Infillings.** `Preprint`

    *Daniel Rose, Vaishnavi Himakunthala, Andy Ouyang, Ryan He, Alex Mei, Yujie Lu, Michael Saxon, Chinmay Sonar, Diba Mirza, William Yang Wang.* [[Paper](https://arxiv.org/abs/2305.02317)] [[Code](https://github.com/dannyrose30/VCOT)], 2023.5

1. **Link-Context Learning for Multimodal LLMs.** `Preprint`

    *Yan Tai, Weichen Fan, Zhao Zhang, Feng Zhu, Rui Zhao, Ziwei Liu.* [[Paper](https://arxiv.org/abs/2308.07891)] [[Code](https://github.com/isekai-portal/Link-Context-Learning)], 20233.8

1. **Chain-of-Table: Evolving Tables in the Reasoning Chain for Table Understanding** `Preprint`

    *Zilong Wang, Hao Zhang, Chun-Liang Li, Julian Martin Eisenschlos, Vincent Perot, Zifeng Wang, Lesly Miculicich, Yasuhisa Fujii, Jingbo Shang, Chen-Yu Lee, Tomas Pfister.* [[Paper](https://arxiv.org/abs/2401.04398)], 2024.1



<h3 id="symbolic">Compositional & Symbolic Approach</h3>



1. **Inferring and Executing Programs for Visual Reasoning.** `ICCV 2017`

    *Justin Johnson, Bharath Hariharan, Laurens van der Maaten, Judy Hoffman, Li Fei-Fei, C. Lawrence Zitnick, Ross Girshick.* [[Project](https://cs.stanford.edu/people/jcjohns/iep/)] [[Paper](https://arxiv.org/abs/1705.03633)] [[Code](https://github.com/facebookresearch/clevr-iep)], 2017.5

1. **Neural-Symbolic VQA: Disentangling Reasoning from Vision and Language Understanding.** `NeurIPS 2018`

    *Kexin Yi, Jiajun Wu, Chuang Gan, Antonio Torralba, Pushmeet Kohli, Joshua B. Tenenbaum.* [[Project](http://nsvqa.csail.mit.edu)] [[Paper](https://arxiv.org/abs/1810.02338)] [[Code](https://github.com/kexinyi/ns-vqa)], 2018.10

1. **Visual Programming: Compositional visual reasoning without training.** `CPVR 2023`

    *Tanmay Gupta, Aniruddha Kembhavi.* [[Project](https://prior.allenai.org/projects/visprog)] [[Paper](https://arxiv.org/abs/2211.11559)] [[Code](https://github.com/allenai/visprog)], 2022.11

1. **ViperGPT: Visual Inference via Python Execution for Reasoning.** `Preprint`

    *Dídac Surís, Sachit Menon, Carl Vondrick.* [[Project](https://viper.cs.columbia.edu/)] [[Paper](https://arxiv.org/abs/2303.08128)] [[Code](https://github.com/cvlab-columbia/viper)], 2023.3

1. **HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in HuggingFace.** `Preprint`

    *Yongliang Shen, Kaitao Song, Xu Tan, Dongsheng Li, Weiming Lu, Yueting Zhuang.* [[Paper](https://arxiv.org/abs/2303.17580)] [[Code](https://github.com/microsoft/JARVIS)], 2023.3

1. **Chameleon: Plug-and-Play Compositional Reasoning with Large Language Models.** `Preprint`

    *Pan Lu, Baolin Peng, Hao Cheng, Michel Galley, Kai-Wei Chang, Ying Nian Wu, Song-Chun Zhu, Jianfeng Gao.* [[Project](https://chameleon-llm.github.io/)] [[Paper](https://arxiv.org/abs/2304.09842)] [[Code](https://github.com/lupantech/chameleon-llm)], 2023.4

1. **Woodpecker: Hallucination Correction for Multimodal Large Language Models.** `Preprint`

    *Shukang Yin, Chaoyou Fu, Sirui Zhao, Tong Xu, Hao Wang, Dianbo Sui, Yunhang Shen, Ke Li, Xing Sun, Enhong Chen.* [[Paper](https://arxiv.org/abs/2310.16045)] [[Code](https://github.com/BradyFU/Woodpecker)], 2023.10

1. **MM-VID: Advancing Video Understanding with GPT-4V(ision).** `Preprint`

    *Kevin Lin, Faisal Ahmed, Linjie Li, Chung-Ching Lin, Ehsan Azarnasab, Zhengyuan Yang, Jianfeng Wang, Lin Liang, Zicheng Liu, Yumao Lu, Ce Liu, Lijuan Wang.* [[Project](https://multimodal-vid.github.io/)] [[Paper](https://arxiv.org/abs/2310.19773)] [[Demo](https://multimodal-vid.github.io/#video-demos)], 2023.10



 ## Benchmark



- **[SCIENCEQA](https://arxiv.org/abs/2209.09513)**  Multimodal multiple choice questions with diverse science topics and annotations of their answers with corresponding lectures and explanations.
- **[ARO](https://arxiv.org/abs/2210.01936)**  Systematically evaluate the ability of VLMs to understand different types of relationships, attributes, and order.
- **[OK-VQA](https://arxiv.org/abs/1906.00067)**  Visual question answering that requires methods which can draw upon outside knowledge to answer questions.
- **[A-OKVQA](https://arxiv.org/abs/2206.01718)**  Knowledge-based visual question answering benchmark.
- **[NExT-QA](https://arxiv.org/abs/2105.08276)**  Video question answering (VideoQA) benchmark to advance video understanding from describing to explaining the temporal actions.
- **[GQA](https://arxiv.org/abs/1902.09506)**  Compositional questions over real-world images.
- **[VQA](https://arxiv.org/abs/1505.00468)**  Questions about images that require an understanding of vision, language and commonsense knowledge.
- **[VQAv2](https://arxiv.org/abs/1612.00837)**  2nd iteration of the Visual Question Answering Dataset (VQA).
- **[TAG](https://arxiv.org/abs/2208.01813)** Questions that require understanding the textual cues in an image.
- **[Bongard-HOI](https://arxiv.org/abs/2205.13803)** Visual reasoning benchmark on compositional learning of human-object interactions (HOIs) from natural images.
- **[ARC](https://arxiv.org/abs/1911.01547)**  General artificial intelligence benchmark, targetted at artificially intelligent systems that aim at emulating a human-like form of general fluid intelligence.


 
 ## Other Useful Resources
 
 
 
 - **[salesforce/LAVIS](https://github.com/salesforce/LAVIS)**  One-stop Library for Language-Vision Intelligence.
 
 
 
 ## Other Awesome Lists



- **[LLM-Reasoning-Papers](https://github.com/atfortes/LLM-Reasoning-Papers)**  Collection of papers and resources on Reasoning in Large Language Models, including Chain-of-Thought, Instruction-Tuning, and others.
- **[Chain-of-ThoughtsPapers](https://github.com/Timothyxxx/Chain-of-ThoughtsPapers)**  A trend starts from "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models".
- **[Prompt4ReasoningPapers](https://github.com/zjunlp/Prompt4ReasoningPapers)**  Repository for the paper "Reasoning with Language Model Prompting: A Survey".
- **[Deep-Reasoning-Papers](https://github.com/floodsung/Deep-Reasoning-Papers)**  Recent Papers including Neural Symbolic Reasoning, Logical Reasoning, Visual Reasoning, planning and any other topics connecting deep learning and reasoning.



## Contributing



- Add a new paper or update an existing paper, thinking about which category the work should belong to.
- Use the same format as existing entries to describe the work.
- Add the abstract link of the paper (`/abs/` format if it is an arXiv publication).

**Don't worry if you do something wrong, it will be fixed for you!**

### Contributors

<a href="https://github.com/atfortes/Awesome-Multimodal-Reasoning/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=atfortes/Awesome-Multimodal-Reasoning" />
</a>
