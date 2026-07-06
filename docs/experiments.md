# Experiments

This file tracks experiment ideas for improving and evaluating the GPT poetry model.

## Baseline runs

- Train with the original Petrarch sonnet corpus.
- Save generated samples at fixed checkpoints.
- Record training loss and validation loss if a validation split is available.

## Sampling settings

Try generating text with different decoding settings:

- greedy decoding
- temperature sampling at 0.7, 1.0, and 1.2
- top-k sampling
- fixed prompt vs empty prompt generation

## Evaluation notes

Qualitative evaluation matters for a poetry model. Useful questions:

- Does the output preserve Italian vocabulary?
- Does it repeat too much?
- Does punctuation look natural?
- Does the generated text resemble sonnet-style phrasing?
- Does increasing temperature improve creativity or create noise?

## Future improvements

- Add a script for sample generation.
- Add a small config file for hyperparameters.
- Add saved example outputs.
- Add reproducibility notes for the Colab workflow.
