# Graph Neural Network for Predicting Network Per-Flow Delays on Real-Time Data 
Jenny Mao

Using RouteNet-F to predict network per-flow delays on Real Traffic Traces. Based off of work done by the wonderful team: 

M. Ferriol-Galmés et al., "RouteNet-Fermi: Network Modeling With Graph Neural Networks," in IEEE/ACM Transactions on Networking, doi: 10.1109/TNET.2023.3269983.


## Installation and Evaluation 

**Recommended: Python 3.7**

You can install all the dependencies by running the following commands.
```
pip install -r requirements.txt
```

## Download the data
You can download the datasets here:
- [Real Traces: SND and MAWI Dataset](https://bnn.upc.edu/download/dataset-v6-real-traces/)
- [FatTree16 Dataset](https://bnn.upc.edu/download/dataset-v6-fat-tree-16/)
- [FatTree64 Dataset](https://bnn.upc.edu/download/dataset-v6-fat-tree-64/)
- [FatTree128 Dataset](https://bnn.upc.edu/download/dataset-v6-fat-tree-128/)

## Training and Validation
If you want to train the model, you can use the following command:
```
python main.py
```

If everything has been done correctly, you should see the following output:

```
Starting training from scratch...
Epoch 1/200
36/4000 [..............................] - ETA: 3:06 - loss: 156.5287
```

Finally, the models will be saved in a `ckp_dir` directory. 

## Prediction
You can  use the following command to predict the metrics with a trained model:
```
python predict.py
```
