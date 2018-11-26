# Graph Convolutional Nets
Graph Convolutional Neural Networks for Theano based on [(kpif et al.)](https://arxiv.org/abs/1609.02907) for classification on the baseline datasets considered in their paper. These datasets are included in the repository in the data folder.

## Dependencies
* theano
* networkx (to unpack the dataset)

## Running the code(demo)

To train the model, simple do
```bash
python main.py
```

This will save a model after every 500 iterations and also test the model on the test dataset. A saved model can be loaded using the --lm option as

```bash
python main.py --lm=$NameSavedModel
```

Finally to test a saved model it can be done with the --t flag as.

```bash
python main.py --lm=$NameSavedModel --t=0
```

The model achieves accuracy on the Cora Dataset


| Dataset | Accuracy |
| ----- | -----|
| Cora | 80.5 | 
