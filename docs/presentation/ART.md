# ART

## Slide 1

### Adversarial Robustness Toolbox

- Developed originally by IBM
- Part of the Linux Foundation
- Targeted against ML models
- Integrated in Counterfit
- Not to be confused with Garak's ART (Auto Red-Team)

## Slide 2

### Capabilities & Attacks

- Wide range of attacks to be run
- TODO: Add a visual representation of all the attacks that can be run

## Slide 3

### Components

- Estimators
  - Wrappers around models
- Metrics
  - Robustness metrics
    - i.e: CLEVER [Weng et al., 2018](https://arxiv.org/abs/1801.10578)
  - Certification
  - Verification
- Blue-teaming (defences)

## Slide 4

### Personal experience

- More or less hard to set up
- Obsolete notebooks
- Unpinned dependencies!
- Requires moderate to great knowledge of datascience
- Lack of standarization
- Would be interesting to create a benchmarkç
  - Difficult because the many kind of models that addresses
- but... Extremely powerful and versatile!

## Slide 5

### Example

- Database reconstruction attack
  - Attackers analyze the model's responses to carefully crafted inputs or utilize public aggregate information to infer individual data points.
- `diffprivlib`
  - library by IBM that include defences for model training
- Steps:
  1. Train a model with and without defences (private gaussian naive bayes classifier)
  2. Delete one column of inputs and outcomes
  3. Reconstruct the data
  4. Calculate RMSE between the reconstructed data and the original to assert how efficient the attack was
