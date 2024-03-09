# Overview
This repo is dedicated to exploring the field of Representation Learning (RepL) with a specific focus on Reinforcement Learning (RL) and Causal Inference. Our goal is to build a comprehensive resource that integrates our latest research and practical implementations.

[Website] [RL-REP: Representation-based Reinforcement Learning](https://haotiansun14.github.io/rl-rep-page/)

## Representation-based Reinforcement Learning
This repo contains implementations for RL with:
- Latent Variable Representations (LV), as outlined in [1].
- Contrastive Representations (CTRL), as described in [2].
- Multi-step Latent Variable Representation $\mu$LV-Rep, as outlined in [3].

### Directory
- `agent` hosts implementation files for various agents, including the Soft Actor-Critic baseline (`sac`), SAC with Latent Variable (`vlsac`), SAC with Contrastive Representations (`ctrlsac`), and DrQv2 with Multi-step Latent Variable Representation (`mulvdrq`).
- `networks` contains base implementations for critics, policy networks, variational autoencoders (VAE), and more.
- `utils` comprises replay buffers and several auxiliary functions.

### Run
Execute the `main.py` script with your preferred arguments, such as `--alg` for algorithm type, `--env` for environment, and so on.

Example usage: `python main.py --alg vlsac --env HalfCheetah-v3`.

### References
[1] [Ren, Tongzheng, Chenjun Xiao, Tianjun Zhang, Na Li, Zhaoran Wang, Sujay Sanghavi, Dale Schuurmans, and Bo Dai. "Latent variable representation for reinforcement learning." arXiv preprint arXiv:2212.08765 (2022).](https://arxiv.org/abs/2212.08765)

[2] [Zhang, Tianjun, Tongzheng Ren, Mengjiao Yang, Joseph Gonzalez, Dale Schuurmans, and Bo Dai. "Making linear mdps practical via contrastive representation learning." In International Conference on Machine Learning, pp. 26447-26466. PMLR, 2022.](https://arxiv.org/abs/2207.07150)

[3] [Hongming Zhang and Tongzheng Ren and Chenjun Xiao and Dale Schuurmans and Bo Dai. "Efficient Reinforcement Learning from Partial Observability." arXiv preprint arXiv:2311.12244 (2024).](https://arxiv.org/abs/2311.12244)

If you find our work helpful, please consider citing our paper:
```
@misc{ren2023latent,
      title={Latent Variable Representation for Reinforcement Learning}, 
      author={Tongzheng Ren and Chenjun Xiao and Tianjun Zhang and Na Li and Zhaoran Wang and Sujay Sanghavi and Dale Schuurmans and Bo Dai},
      year={2023},
      eprint={2212.08765},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
```
@misc{zhang2022making,
      title={Making Linear MDPs Practical via Contrastive Representation Learning}, 
      author={Tianjun Zhang and Tongzheng Ren and Mengjiao Yang and Joseph E. Gonzalez and Dale Schuurmans and Bo Dai},
      year={2022},
      eprint={2207.07150},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
```
@misc{zhang2024efficient,
      title={Efficient Reinforcement Learning from Partial Observability}, 
      author={Hongming Zhang and Tongzheng Ren and Chenjun Xiao and Dale Schuurmans and Bo Dai},
      year={2024},
      eprint={2311.12244},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```