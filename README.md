# Denoising Diffusion Probabilistic Models

Experiments run on Google Cloud TPU v3-8.

Requires TensorFlow 1.15 and Python 3.5, and these dependencies for CPU instances (see `requirements.txt`):
```
pip3 install fire
pip3 install scipy
pip3 install pillow
pip3 install tensorflow-probability==0.8
pip3 install tensorflow-gan==0.0.0.dev0
pip3 install tensorflow-datasets==2.1.0
```

The training and evaluation scripts are in the `scripts/` subdirectory.
The commands to run training and evaluation are in comments at the top of the scripts.
Data is stored in GCS buckets. The scripts are written to assume that the bucket names are of the form `gs://mybucketprefix-us-central1`; i.e. some prefix followed by the region.
The prefix should be passed into the scripts using the `--bucket_name_prefix` flag.

Models and samples can be found at: https://www.dropbox.com/sh/pm6tn31da21yrx4/AABWKZnBzIROmDjGxpB6vn6Ja

## Citation
If you find our work relevant to your research, please cite:
```
@article{ho2020denoising,
    title={Denoising Diffusion Probabilistic Models},
    author={Jonathan Ho and Ajay Jain and Pieter Abbeel},
    year={2020},
    journal={arXiv preprint}
}
```
