# Natural Language Inference

## Prerequisite

* Python 3.5

* Tensorflow 1.8

* numpy

* pickle

* logging

## Experiments

To reproduce the results of our network, run the following command

python hyp_rnn.py --base_name='' --dataset='SNLI' --inputs_geom='hyp' -word_dim=5 --word_init_avg_norm=0.001   --cell_type='gru' --cell_non_lin='id'  --sent_geom='hyp' --bias_geom='hyp' --ffnn_geom='hyp' --ffnn_non_lin='id' --additional_features='dsq'  --dropout=1.0 --before_mlr_dim=5 --mlr_geom='hyp'  --reg_beta=0.0  --hyp_opt='rsgd' --lr_ffnn=0.01 --lr_words=0.1 --burnin='n' --proj_eps=1e-5 --batch_size=64 --root_path=./ --point_to_hyperplane_distance='syms'

## Acknowledgement

The code in this repository is based on this open source implementation ([link](https://github.com/dalab/hyperbolic_nn)). If you use our code, please consider citing the paper [Hyperbolic Neural Network](https://arxiv.org/pdf/1805.09112).
