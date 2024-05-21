# ProofFrog-KEMs

ProofFrog primitives, schemes, games and proofs around key encapsulation mechanisms (KEMs).

## Setup

You can follow the [Proof Frog instructions](https://prooffrog.github.io/#installation), which at
time of writing allows:

```
pipx install proof_frog

```

I recommend [pipx](https://pipx.pypa.io/stable/) as it does the isolated Python environments
juggling for you and is available on most platforms by their predominant package manager.

If you need a bleeding edge version that hasn't been published to PyPi yet, you can build and
install it yourself:

```
git clone https://github.com/ProofFrog/ProofFrog
cd ProofFrog
pipx install -e .
```

Once you have a `proof_frog` command available, you can parse and prove stuff in this repo like so:

```
git clone https://github.com/dconnolly/ProofFrog-KEMs
cd ProofFrog-KEMs
proof_frog parse game Games/IND_CCA.game
```

Proof Frog doesn't quite work if you execute it from a location where the relative paths of the
imports don't make sense, so it's best to just run it from the root of the repo.


