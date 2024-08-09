# Graph-Jigsaw Conditioned Diffusion Model for Skeleton-based Video Anomaly Detection

PyTorch implementation of GiCISAD.

## Citation

You can find the preprint of our paper on [arXiv](https://arxiv.org/abs/2403.12172).

Please cite our paper if you use the results of our work.

```
@article{karami2024graphjigsawconditioneddiffusionmodel,
      title={Graph-Jigsaw Conditioned Diffusion Model for Skeleton-based Video Anomaly Detection}, 
      author={Ali Karami and Thi Kieu Khanh Ho and Narges Armanfard},
      year={2024},
      eprint={2403.12172},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2403.12172}, 
}
```


# Instructions for Running the Code

To train the model with all necessary dependencies, execute the script GiCiSAD.sh. 
This script includes the command:
python train.py --config config/Avenue/GiCiSAD_train.yaml

To train the model using different datasets, the command format is as follows:
python train.py --config config/[Avenue/UBnormal/STC]/{config_name}.yaml

After training, you can test the model using the following command:
python eval.py --config checkpoints/HR-Avenue/train_experiment/config.yaml

This command uses the configuration from a specific training experiment, 
identified by the path to its configuration file within the checkpoints directory.

Certain segments of the code have been derived from external sources. 
Due to the requirements of the double-blind review process, these sources were not cited in the initially submitted source code.
We assure you that all external contributions will be duly cited in the final, 
camera-ready version of the paper to ensure full transparency and to address any concerns regarding plagiarism.



