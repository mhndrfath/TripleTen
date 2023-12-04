# Goal:
Building a machine learning model that predicts the amount of gold recovered from the extraction process so as to optimize production

# Data Description
Technological Process:
- `Rougher feed` — raw material for the flotation process
- `Rougher additions` (or reagent additions) — reagents for flotation: Xanthate, Sulphate, Depressant
- `Xanthate` — flotation activator or activator
- `Sulphate` — sodium sulfide, specifically for this process
- `Depressant` — sodium silicate
- `Rougher process` — flotation
- `Rougher tails` — product residue
- `Float banks` — flotation units
- `Cleaner process` — purification
- `Rougher Au` — a coarser gold concentrate
- `Final Au` — final gold concentrate

Parameters of the Available Stages
- `air amount` — air volume
- `fluid levels`
- `feed size` — the size of the feed particles
- `feed rate`

## Feature Naming

Here is how to give names to existing features:

[stage].[parameter_type].[parameter_name]

Example: rougher.input.feed_ag

Possible values for [stage]:
- `rougher` — flotation
- `primary_cleaner` — first cleanup
- `secondary_cleaner` — secondary cleaning
- `final` — final characteristic

Possible values for [parameter_type]:
- `input` — raw material parameters
- `output` — product parameters
- `state` — parameters indicating the characteristics of the current stage
- `calculation` — calculation of characteristics

# Libraries
*pandas, matplotlib, numpy, sklearn*

# Content
- Introduction
- Data Overview
- Data Pre-Processing
- Data Analysis
- Modelling
- General Conclusion
