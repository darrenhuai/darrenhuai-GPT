# Model Notes

This project follows the core idea behind GPT-style autoregressive language modeling: predict the next token from the tokens that came before it.

## Dataset

The training data is based on Petrarch's Italian sonnets. A narrow poetry corpus makes the model easier to inspect because generated samples can be compared against a consistent style, meter, and vocabulary.

## Training objective

The model learns by minimizing next-token prediction loss. During training, the input sequence is shifted against the target sequence so that each position predicts the following token.

## Generation

Text generation starts from a prompt or seed token sequence. At each step, the model predicts a probability distribution over the next token, samples or selects one token, appends it to the context, and repeats.

## Useful experiments

- Compare greedy decoding with temperature sampling.
- Track training loss over time.
- Generate samples from the same prompt at different temperatures.
- Compare short-context and long-context outputs.
- Inspect whether generated text preserves sonnet-like vocabulary and structure.
