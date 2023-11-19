# Experiment Patch Sets for Data Collections of PoPETs 2024.2 "MixMatch" Paper

This repository holds the Nym patch sets to transform the Nym repository at a particular version into the state for a particular experiment that we conduct as part of our PoPETs 2024.2 paper "MixMatch: Flow Matching for Mixnet Traffic". Each subfolder in this repository represents one of the experiments `baseline`, `no-cover`, `low-delay`, `high-delay`, and `live-nym`. (The final dataset, `two-to-one`, that we construct and analyse in the paper is built ad-hoc from `baseline` in the drift and statistical classifier directly and thus not present in this repository.) Please see each subfolder's respective `README.md` for a brief description of the experiment's configuration details.

**Please mind:** This repository is part of a larger list of repositories that make up the artifacts of our paper. It takes a specific place in the data collection process and thus might not provide you enough information on its own to be useful to you. Please also read through the documentation in our [main paper repository](https://github.com/mixnet-correlation/mixmatch-flow-matching-for-mixnet-traffic_popets-2024-2).

While we use keyword names for our experiments in the paper, we initially used `exp0X` names instead. For compatibility with our existing source code, we are keeping the original naming scheme in this repository. Please refer to below translation when going from experiment name in the paper to experiment name in this repository:
* `baseline` => [`exp01_nym-binaries-1.0.2_static-http-download`](./exp01_nym-binaries-1.0.2_static-http-download/)
* `no-cover` => [`exp02_nym-binaries-1.0.2_static-http-download_no-client-cover-traffic`](./exp02_nym-binaries-1.0.2_static-http-download_no-client-cover-traffic/)
* `low-delay` => [`exp05_nym-binaries-1.0.2_static-http-download_shorter-mix-delay`](./exp05_nym-binaries-1.0.2_static-http-download_shorter-mix-delay/)
* `high-delay` => [`exp06_nym-binaries-1.0.2_static-http-download_longer-mix-delay`](./exp06_nym-binaries-1.0.2_static-http-download_longer-mix-delay/)
* `live-nym` => [`exp08_nym-binaries-v1.1.13_static-http-download`](./exp08_nym-binaries-v1.1.13_static-http-download/)


### Usage of This Repository

Unless of independent analysis interest, this repository *should* only be used as part of the Isolated Setup / Live-Network Setup orchestration. It will be downloaded automatically when either of the setups is deployed to collect datasets. Please refer to the [Isolated Setup repository](https://github.com/mixnet-correlation/data-collection_2_isolated-setup) and the [Live-Network Setup repository](https://github.com/mixnet-correlation/data-collection_3_live-network-setup) for usage instructions.
