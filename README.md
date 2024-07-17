# Trajectory Quantizer/Tokenizer

Jupyter notebook contains the code to implement quantizer from the paper [MotionLM](https://arxiv.org/abs/2309.16534).

Here although the implementation follows the native structure as described in the paper. The verlet Integration is missing.

## Environment Setup

1. Follow the setup instructions from [AV2 repo](https://argoverse.github.io/user-guide/getting_started.html) to get the necessary packages installed.
2. Using the pip version is the easiest as it uses rust. Before using the `pip install -e /path/to/root/dir/of/the/project` ensure you run `cargo update` from the root dir to pull all the changes from remote.
3. For any issues related to installation follow this [link](https://github.com/argoverse/av2-api/issues/211#issuecomment-1630851880).

## Creating a symlink

 ```bash
$ mkdir data/ && cd data && ln -s ~/path/to/local/mount/ 2_av2
 ```
This command allows you to create a softlink to the original dataset which might be located in a different mount. This is recommended and mandatory to ensure that the rest of the scripts work as expected.

## TODO

- [ ] Implement Verlet Integration to reduce the bin size.
