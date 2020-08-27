# CUPL-master
This is a pytorch implementation of our paper: "Learning Complete User Preferences for Cross Domain Recommendation"  

You can access the paper through:  

**Running Tips**  
This folder contains the thhree datasets used in our paper and the codes of our CUPL model. Specifically, main_my.py is our model and the other four main_xxx.py files are four variants of CUPL in the abalation study of our paper.  

1. Requirements:  
pytorch==;  

2. Run the codes with the following commands on different datasets (amazon means "Movie & Book", amazon2 means "Movie & Music" and amazon3 means "Music & Book").  

**on Movie & Book dataset**  
CUDA_VISIBLE_DEVICES=gpu_num python main_my.py --dataset=amazon --reg=5.0  

**on Movie & Music dataset**  
CUDA_VISIBLE_DEVICES=gpu_num python main_my.py --dataset=amazon2 --reg=0.5  

**on Music & Book dataset**  
CUDA_VISIBLE_DEVICES=gpu_num python main_my.py --dataset=amazon3 --reg=1.0  

In this way, you can get he results. Besides, if you want to run the variants of CUPL, just follow the same way while with different main files.  
If you find the codes are useful, please cite our paper.

@article{xu2020learning,  
  title={POG: Personalized Outfit Generation for Fashion Recommendation at Alibaba iFashion},  
  author={Xu Chen, Ya Zhang, Ivor Tsang, Yuangang Pan and Jingchao Su},  
  journal={arXiv preprint arXiv:xxxx.xxxxx},  
  year={2020}  
}  
