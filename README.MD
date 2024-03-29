
# Fast and Reliable Evaluation of Adversarial Robustness with Minimum-Margin Attack
Hi, this is the pytorch code for MM attack, presented in the ICML2022 paper " Fast and Reliable Evaluation of Adversarial Robustness with
Minimum-Margin Attack". This work is done by  

- Ruize Gao (CUHK), ruizegao@comp.nus.edu.sg / sjtu16.brian.gao@gmail.com
- Jiongxiao Wang (CUHK), 17300180069@fudan.edu.cn
- Kaiwen Zhou (CUHK), kwzhou@cse.cuhk.edu.hk
- Feng Liu (UTS), feng.liu1@unimelb.edu.au  
- Binghui Xie (CUHK), bhxie21@cse.cuhk.edu.hk
- Gang Niu (RIKEN), gang.niu.ml@gmail.com 
- Bo Han (HKBU), bhanml@comp.hkbu.edu.hk    
- James Cheng (CUHK), jcheng@cse.cuhk.edu.hk
# Software
We recommend users to install python via Anaconda (python 3.7.3), which can be downloaded from https://www.anaconda.com/distribution/#download-section.  

Torch: 1.1.0  

Python: 3.7.3  

CUDA: 10.1  

# Compared with Other Attack Methods
If you want to compare MM Attack with other attack methods, please run
```
python mm_attack.py --resume YOUR_MODEL --mode compare
```
You will get the model accuracy and time of all the attack methods mentioned in our paper for comparison.

If you want to compare MM Attack with AutoAttack, please install the auto-attack package  
```
pip install git+https://github.com/fra31/auto-attack
```

Then you can get results of AutoAttack by running  
```
python autoattack_test.py --resume YOUR_MODEL
```

# Use MM Attack Only
If you only want to use MM Attack, please run
```
python mm_attack.py --resume YOUR_MODEL --mode attack --perturb_steps 20 --eps 0.031 --k 3
```
You can choose your own attack steps, epsilon bound and top k classes for attack.

Note: You may need to add proper ways when loading the resume models.

# MM3-F/MM3 Adversarial Training
To use adversarial examples generated by MM Attack for Adversarial Training, please run
1) for using adaptive steps MM Attack to generate adversarial examples
```
python mm_at.py
```
2) for using fixed steps MM Attack to generate adversarial examples
```
python mmu_at.py
```

# Citation
If you are using this code for your own researching, please consider citing
```
@inproceedings{gao2022fast,
  title={Fast and Reliable Evaluation of Adversarial Robustness with Minimum-Margin Attack},
  author={Gao, Ruize and Wang, Jiongxiao and Zhou, Kaiwen and Liu, Feng and Xie, Binghui and Niu, Gang and Han, Bo and Cheng, James},
  booktitle={ICML},
  year={2022}
}
```

# Acknowledgment
RZG, JXW, KWZ, BHX and JC were supported by GRF 14208318 from the RGC of HKSAR. BH was supported by the RGC Early Career Scheme No. 22200720, NSFC Young Scientists Fund No. 62006202, and Guangdong Basic and Applied Basic Research Foundation No. 2022A1515011652. GN were supported by JST AIP Acceleration Research Grant Number JPMJCR20U3, Japan. 


