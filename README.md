# ResGCN

This is a Tensorflow implementation of Residual Graph Convolutional Networks for the tesk of Classification of heterogeneous information networks

## Installation

The source code is beasd on GCN

```bash
python -m pip install -r requirements.txt
```

## Resquirements
* tensorflow == 1.15.0
* networkx

## Run the demo

```bash
git clone https://github.com/youthliuxi/ResGCN.git
```

## Data

In order to use your own data, you have to provide 
* an N by N adjacency matrix (N is the number of nodes), 
* an N by D feature matrix (D is the number of features per node), and
* an N by E binary label matrix (E is the number of classes).

Have a look at the `readData()` function in `utils.py` for an example.

You can specify a dataset as follows:

```bash
python train.py --dataset DBLP2
```

(or by editing `train.py`)