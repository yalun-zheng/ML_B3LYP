<img src="https://github.com/user-attachments/assets/50c452f8-c765-4ae2-8fe5-96a9fabc9e24" alt="img" width="600" height="450">  

#### Step 1
Clone this repository into your device. Run  
```
git clone https://github.com/yalun-zheng/ML_B3LYP.git
```  
or
```
git clone git@github.com:yalun-zheng/ML_B3LYP.git
```      
Assume that the repository is cloned in /path_to_code/ML_B3LYP, then assign this path in cfg.yaml and in run.sh, separately, as follows.   
In cfg.yaml, change the first line homepath: /mnt/c/Users/yalun/Desktop/ML_B3LYP with  
```
homepath: /path_to_code/ML_B3LYP
```     
Also in run.sh, change the first line cd /mnt/c/Users/yalun/Desktop/ML_B3LYP with  
```
cd /path_to_code/ML_B3LYP
```

#### Step 2
Install some necessary packages.  
```numpy==1.26.0  
pyscf==2.3.0
opt_einsum
yaml
ml_collections
torch  
matplotlib
pandas
```
Make sure directories named with subsets name like `/path_to_code/ML_B3LYP/data/pkl/G2/`, `/path_to_code/ML_B3LYP/data/pkl/test/` or `/path_to_code/ML_B3LYP/data/pkl/other_dataset_name/`  are made.
#### Step 3
Run the script run.sh to train valid or test a model.  
```
sh run.sh
```
The validation and test results using the default model will be saved in valid.csv and test.csv    

#### Note  
By editing cfg.yaml and giving the corresponding xyz files, you can validate/test any structure using any model you trained.
