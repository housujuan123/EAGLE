# EAGLE Network: A Novel Incremental Learning Framework for Detecting Unknown Logos in Open-World Environments

Logo detection is an important task in the field of computer vision, including extensive applications in intelligent transportation, advertising and entertainment. However, real-world logo detection requires adressing unknown logo samples. Therefore, we define the Open-world Logo Detection (OWLD) task. In open-world settings, it necessitates not only precise classification of known classes but also the recognition of unknown classes. Additionally, it requires leveraging deep learning's robust feature learning capabilities to progressively achieve incremental learning of new logo classes. Due to potential problems such as partial occlusion, scale variation, and rotational skew in logo images, some open-world object detection methods perform poorly in logo detection, exhibiting low accuracy and apparent forgetting. To address these challenges, we propose an AttEntion-guided TAsk Queries Generation DecoupLing and Task AdaptivE Network (EAGLE) for OWLD. Specifically, we designed an attention-guided task queries generation decoupling (AQD) module, which shares the self-attention layer in the decoder and decouples the subsequent operations of cross-attention and feedforward neural network into two branches. The location information output by the localization branch is fused with the global features extracted by the shared self-attention layer into class queries to aid classification. Furthermore, we introduce a task-adaptive (TA) module. We propose freezing the parameters of the encoder in the original task and introducing learnable adapter modules to learn the features and data distribution of the new task. This approach helps retain previously learned knowledge when introducing new logo classes, preventing apparent forgetting. Extensive experiments conducted on three public logo datasets demonstrate the efficiency of our proposed method.

# Usage
To train the model, use
" bash run.sh "

# Citation
@inproceedings{10.1145/3688859.3690081,  
author = {Yuan, Zhongming and Xiong, Hao and Hou, Sujuan},  
title = {EAGLE Network: A Novel Incremental Learning Framework for Detecting Unknown Logos in Open-World Environments},  
year = {2024},  
isbn = {9798400711886},    
publisher = {Association for Computing Machinery},      
address = {New York, NY, USA},      
doi = {10.1145/3688859.3690081},    
booktitle = {Proceedings of the 1st on Continual Learning Meets Multimodal Foundation Models: Fundamentals and Advances},    
pages = {23–30},    
numpages = {8},    
keywords = {incremental learning, open-world logo detection, task queries generation, task-adaptive},    
location = {Melbourne VIC, Australia},    
series = {ACMMM CL'24}    
}

