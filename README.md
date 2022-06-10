# CRL
Improve of the research paper [Consistent Representation Learning for Continual Relation Extraction](https://arxiv.org/abs/2203.02721) (Findings of ACL 2022)

## Framwork of consistent representation learning

Memory Replay Architecture

<div align="center">
<img src=figs/crl.png width=80% />
</div>

## Dependencies

Use anaconda to create python environment:

> conda create --name yourname python=3.8 \
> conda activate yourname

Install Pytorch (suggestions>=1.7) and related environmental dependencies:

> pip install -r requirements.txt


### Run the Code

> python run_continual.py --dataname FewRel

### Our improve
Version 1: Using raw prototypes
> python run_continual.py --dataname FewRel --protos_raw True

Version 2: Multitask training with pareto in memory
> python run_continual.py --dataname FewRel --multitask True

