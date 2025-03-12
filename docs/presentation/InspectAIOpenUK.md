# InspectAIOpenUK

## Slide 1

### Inspect OpenUK

- Benchmark for LLM models with many evaluations
- Just two probes related to security
  - Harm
  - Hazardous knowledge (Unlearning)

## Slide 2

### Components

- Datasets
  - Table with `input` and `target` (grading guidance)
- Solvers
  - Accepts inputs and provide a result. The most elemental solver is `generate()` (which just calls the model)
  - Other solvers may add a bit to the input, for example performing prompt engineering
- Scorers
  - Evaluates the output of solvers

## Slide 3

### Personal opinion & Other

- Robust and easy to use
- Up to date withd dependencies
- 813 stars in Github
- Not the most exhaustive security tool but it also evaluates performance

## Slide 4

### Example

![Alt text](image.png)

## Slide 5

### Example

![Alt text](image-1.png)

### Errors

- Failed with phi-2 `2025-03-11T18-50-22+00-00_agentharm_3DH86fPyyzL7zjzexB2XsY.eval`
