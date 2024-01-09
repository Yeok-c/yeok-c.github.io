---
title: "SAPIEN Open-Source Manipulation Skill (ManiSkill) 2 Challenge by UCSD (2023)"
excerpt: "Passionate about learning-based robotics, I participated and won 2nd runner-up the ManiSkill2 Challenge hosted by Prof Haosu’s lab at UC San Diego.<br/><img src='/images/portfolio/rss_3.jpg' width='600'>"
collection: portfolio
---

Passionate about learning-based robotics, I participated and won 2nd runner-up the ManiSkill2 Challenge hosted by Prof Haosu’s lab at UC San Diego. ManiSkill2 [1] is a benchmark for generalizable learning-based algorithms in robotics across a variety of tasks, manipulating both rigid and soft objects. My implementation uses a pretrained PointNet++ backbone on a learned agent trained with Demonstration Augmented Policy Gradients (DAPG) for tasks where simulation is fast, and behavioural cloning for tasks where simulation is expensive. I also experimented with privileged state and multi-camera information, which seems to be quite popular in recent papers, to ensure convergence. 

<img src='/images/portfolio/rss_5.png' width='600'>

Screenshot from the official ManiSkill2 Challenge Website

I was invited attend the Interdisciplinary Exploration of Generalizable Manipulation Policy Learning Workshop at RSS Conference 2023, where I had the privilege of listening to and engaging in discussions with esteemed professors who have been my source of inspiration for years. I met the one and only Andy Zeng who pioneered the foundation of modern robotic pick-and-place operations with his work in grasp affordances in 2017 and witness his convincing argument on the integration of LLMs in robotics to overcome fundamental limitations of data-driven robotics. I also met Prof. Joseph J Lim and Dr. Youngwoon whose work is fundamental in long-horizon tasks in reinforcement learning, Professor Shan Luo whose work in simulating tactile sensors pave the way for safe collaborative robots. Moreover, I had the pleasure of connecting with brilliant minds like Dr Yashraj Narang from Nvidia, Dr. Xinyu Lin from UCB, along with other professors, postdocs and PhD students I encountered during this remarkable journey. I'm very grateful for the enlightening conversations and invaluable advice towards embarking on my path as a Ph.D. student. 

<img src='/images/portfolio/rss_1.jpg' width='600'>

Award giving ceremony at the RSS workshop

<img src='/images/portfolio/rss_2.jpg' width='600'>

Discussion panel with (left to right) Prof. Shan Luo, Andy Zeng, Pietro Mazzaglia, Dr. Xinyu Lin, Prof. Hao Su, and Prof. Joseph J Lim.

<img src='/images/portfolio/rss_4.jpg' width='600'>

Got a personal picture with Andy Zeng!

<br>

Here's my what I gathered after the entire day: 

Many large computer-science-focused robotic groups, including the Google Brain and Google Deepmind teams, seem focused on developing vision-language-action transformers as high-level planners (i.e., ‘foundational models’). Beyond utilizing the obvious natural language, planning and reasoning capabilities of LLMs in robotics [2-12], the scale and nuance of language datasets to complement demonstration-based robotic datasets is essential for ‘true’ zero-shot learning [5, 8, 9, 12, 13], better leverage or transfer-learn skill-based policies [14-16], and perhaps may one day remove implicit biases. Furthermore, modelling high-level robotic tasks as transformer token sequences instead of MDPs also appears to have benefits [17-19]. Personally I believe generalizable high-level planners combined with reliable low-level policies such as RL, MPC, LLM-generated motion primitives [20-22] (or a combination of them) will already be capable of solving most of today’s robotic manipulation benchmarks, which consist of mostly pick-place-push-pull tasks. 

However, most real-world tasks concern objects that have complicated contact physics. Tasks such as holding vegetables in a bundle, while cutting them, or folding clothes require better dynamic models and tactile sensors than what we have today. Hence another major research direction is to develop better representations for spatial (shape, pose in clutters, etc.) and temporal dynamic (state-action transitions) of objects in manipulation tasks. 

Lastly, From what I understand, besides using pre-trained vision models as backbones, researchers have approached the topic by further pre-training with masked vision [23-25], pre-training with videos [26-29], use reconstructed views to provide a spatially consistent representation [17, 30], or reconstruct neural representations of scenes [31, 32]. I believe developing strong representations for robotic learning is essential to the real challenges in robotics, such as handling tools or working in unstructured environments. 


[1]	Gu, Jiayuan, et al. "Maniskill2: A unified benchmark for generalizable manipulation skills." arXiv preprint arXiv:2302.04659, 2023

[2]	J. Wu et al., "Tidybot: Personalized robot assistance with large language models," arXiv preprint arXiv:2305.05658, 2023.

[3]	S. Huang, Z. Jiang, H. Dong, Y. Qiao, P. Gao, and H. Li, "Instruct2Act: Mapping Multi-modality Instructions to Robotic Actions with Large Language Model," arXiv preprint arXiv:2305.11176, 2023.

[4]	D. Driess et al., "Palm-e: An embodied multimodal language model," arXiv preprint arXiv:2303.03378, 2023.

[5]	W. Huang, P. Abbeel, D. Pathak, and I. Mordatch, "Language models as zero-shot planners: Extracting actionable knowledge for embodied agents," in International Conference on Machine Learning, 2022: PMLR, pp. 9118-9147. 

[6]	X. Zhao, M. Li, C. Weber, M. B. Hafez, and S. Wermter, "Chat with the environment: Interactive multimodal perception using large language models," arXiv preprint arXiv:2303.08268, 2023.

[7]	B. Lin, Y. Zhu, Z. Chen, X. Liang, J. Liu, and X. Liang, "Adapt: Vision-language navigation with modality-aligned action prompts," in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 15396-15406. 

[8]	Y. Jiang et al., "Vima: General robot manipulation with multimodal prompts," arXiv preprint arXiv:2210.03094, 2022.

[9]	J. Wu et al., "TidyBot: Personalized Robot Assistance with Large Language Models," ArXiv, vol. abs/2305.05658, 2023.

[10]	K. Lin, C. Agia, T. Migimatsu, M. Pavone, and J. Bohg, "Text2Motion: From Natural Language Instructions to Feasible Plans," ArXiv, vol. abs/2303.12153, 2023.

[11]	Y. Guo, Y.-J. Wang, L. Zha, Z. Jiang, and J. Chen, "DoReMi: Grounding Language Model by Detecting and Recovering from Plan-Execution Misalignment," arXiv preprint arXiv:2307.00329, 2023.

[12]	E. Jang et al., "Bc-z: Zero-shot task generalization with robotic imitation learning," in Conference on Robot Learning, 2022: PMLR, pp. 991-1002. 

[13]	T. Brown et al., "Language models are few-shot learners," Advances in neural information processing systems, vol. 33, pp. 1877-1901, 2020.

[14]	F. Ebert et al., "Bridge data: Boosting generalization of robotic skills with cross-domain datasets," arXiv preprint arXiv:2109.13396, 2021.

[15]	Y. Jiang, Q. Gao, G. Thattai, and G. Sukhatme, "Language-Informed Transfer Learning for Embodied Household Activities," arXiv preprint arXiv:2301.05318, 2023.

[16]	S. Karamcheti et al., "Language-driven representation learning for robotics," arXiv preprint arXiv:2302.12766, 2023.

[17]	M. Shridhar, L. Manuelli, and D. Fox, "Perceiver-actor: A multi-task transformer for robotic manipulation," in Conference on Robot Learning, 2023: PMLR, pp. 785-799. 

[18]	A. Goyal, J. Xu, Y. Guo, V. Blukis, Y.-W. Chao, and D. Fox, "RVT: Robotic View Transformer for 3D Object Manipulation," arXiv preprint arXiv:2306.14896, 2023.

[19]	Z. Jia, F. Liu, V. Thumuluri, L. Chen, Z. Huang, and H. Su, "Chain-of-Thought Predictive Control," arXiv preprint arXiv:2304.00776, 2023.

[20]	I. Singh et al., "Progprompt: Generating situated robot task plans using large language models," in 2023 IEEE International Conference on Robotics and Automation (ICRA), 2023: IEEE, pp. 11523-11530. 
[21]	J. Liang et al., "Code as policies: Language model programs for embodied control," in 2023 IEEE International Conference on Robotics and Automation (ICRA), 2023: IEEE, pp. 9493-9500. 

[22]	R. Wang, J. Mao, J. Hsu, H. Zhao, J. Wu, and Y. Gao, "Programmatically Grounded, Compositionally Generalizable Robotic Manipulation," arXiv preprint arXiv:2304.13826, 2023.

[23]	I. Radosavovic, T. Xiao, S. James, P. Abbeel, J. Malik, and T. Darrell, "Real-World Robot Learning with Masked Visual Pre-training," ArXiv, vol. abs/2210.03109, 2022.

[24]	T. Xiao, I. Radosavovic, T. Darrell, and J. Malik, "Masked Visual Pre-training for Motor Control," ArXiv, vol. abs/2203.06173, 2022.

[25]	S. Parisi, A. Rajeswaran, S. Purushwalkam, and A. K. Gupta, "The Unsurprising Effectiveness of Pre-Trained Vision Models for Control," in International Conference on Machine Learning, 2022. 

[26]	K. Shaw, S. Bahl, and D. Pathak, "VideoDex: Learning Dexterity from Internet Videos," in Conference on Robot Learning, 2022. 

[27]	E. Chane-Sane, C. Schmid, and I. Laptev, "Learning Video-Conditioned Policies for Unseen Manipulation Tasks," 2023 IEEE International Conference on Robotics and Automation (ICRA), pp. 909-916, 2023.

[28]	K. Grauman et al., "Ego4d: Around the world in 3,000 hours of egocentric video," in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 18995-19012. 

[29]	S. Nair, A. Rajeswaran, V. Kumar, C. Finn, and A. Gupta, "R3m: A universal visual representation for robot manipulation," arXiv preprint arXiv:2203.12601, 2022.

[30]	A. Zeng et al., "Transporter networks: Rearranging the visual world for robotic manipulation," in Conference on Robot Learning, 2021: PMLR, pp. 726-747. 

[31]	Z. Xue, Z. Yuan, J. Wang, X. Wang, Y. Gao, and H. Xu, "USEEK: Unsupervised SE(3)-Equivariant 3D Keypoints for Generalizable Manipulation," 2023 IEEE International Conference on Robotics and Automation (ICRA), pp. 1715-1722, 2022.

[32]	L. Yen-Chen et al., "MIRA: Mental Imagery for Robotic Affordances," arXiv preprint arXiv:2212.06088, 2022.










