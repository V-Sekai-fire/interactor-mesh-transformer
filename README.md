# interactor-mesh-transformer

Training and test scripts for a text-conditioned transformer that generates triangle meshes, built on the meshgpt-pytorch library.

## What it is for

An autoencoder learns to turn a mesh's triangles into tokens, and a transformer learns to generate those tokens from a text label, so a new mesh can be sampled from a description. The method follows MeshGPT (Siddiqui et al., 2023).

## Building and running

```sh
pip install -r requirements.txt
./start.sh
```

`start.sh` launches transformer training; the autoencoder scripts run with `python`. The scripts read prepared mesh datasets and checkpoints from outside the repository.

## Licence

MIT. See [LICENSE](LICENSE).
