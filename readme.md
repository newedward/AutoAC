# AutoAC: Towards Automated Attribute Completion for Heterogeneous Graph Neural Network
___
code for the paper "Towards Automated Attribute Completion for Heterogeneous Graph Neural Network"

## Dataset
We use datasets recently proposed by [HGB](https://www.biendata.xyz/hgb/).ACM can be found in this repo,DBLP and IMDB can be found  in [HGB](https://www.biendata.xyz/hgb/#/datasets) 

## Quick start
The requirements of the running environment is listed in requirements.txt. After installing the packages run: 
```
bash test_result.sh
```
In test_result.sh ,some commands is given
```
python3 search_retrain.py --dataset=ACM --gnn-model=simpleHGN --searcher_name nasp --cluster-num 12 --patience_search 8 --patience_retrain 30 --shared_ops --use_dmon --dmon_loss_alpha 0.4 --use_5seeds
```
## How to evaluate
After running AutoAc,five submit files will be generated. You can upload them in [this website](https://www.biendata.xyz/competition/hgb-1/) to get results
