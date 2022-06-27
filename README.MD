
# Fast and Reliable Evaluation of Adversarial Robustness with Minimum-Margin Attack
Hi, this is the pytorch code for MM attack, presented in the ICML2022 paper " Fast and Reliable Evaluation of Adversarial Robustness with
Minimum-Margin Attack". This work is done by  

- Ruize Gao (CUHK), sjtu16.brian.gao@gmail.com
- Jiongxiao Wang (CUHK), 17300180069@fudan.edu.cn
- Kaiwen Zhou (CUHK), kwzhou@cse.cuhk.edu.hk
- Feng Liu (UTS), feng.liu1@unimelb.edu.au  
- Binghui Xie (CUHK), bhxie21@cse.cuhk.edu.hk
- Gang Niu (RIKEN), gang.niu.ml@gmail.com 
- Bo Han (HKBU), bhanml@comp.hkbu.edu.hk    
- James Cheng (CUHK), jcheng@cse.cuhk.edu.hk
# Software
We recommend users to install python via Anaconda (python 3.7.3), which can be downloaded from https://www.anaconda.com/distribution/#download-section.  

Most codes require freqopttest repo (interpretable nonparametric two-sample test) to implement ME and SCF tests, which can be installed by  
```
pip install git+https://github.com/wittawatj/interpretable-test
```
Torch: 1.1.0  

Python: 3.7.3  

CUDA: 10.1  

# Citation
If you are using this code for your own researching, please consider citing
```
@article{gao2022fast,
  title={Fast and Reliable Evaluation of Adversarial Robustness with Minimum-Margin Attack},
  author={Gao, Ruize and Wang, Jiongxiao and Zhou, Kaiwen and Liu, Feng and Xie, Binghui and Niu, Gang and Han, Bo and Cheng, James},
  journal={arXiv preprint arXiv:2206.07314},
  year={2022}
}
```

# Acknowledgment
RZG, JXW, KWZ, BHX and JC were supported by GRF 14208318 from the RGC of HKSAR. BH was supported by the RGC Early Career Scheme No. 22200720, NSFC Young Scientists Fund No. 62006202, and Guangdong Basic and Applied Basic Research Foundation No. 2022A1515011652. GN were supported by JST AIP Acceleration Research Grant Number JPMJCR20U3, Japan. 


