# Research Steps
*This markdown is merely for developers to arrange the Research*

## Step 1 Understanding and Document Existing PPO Workflows

Understand existing PPO workflows in mature statistical software and summarize them in Markdown.

For each target, summary should include:
1. The standard workflow identified.
2. The role of each important function or component.
3. The statistical purpose of each step.
4. The inputs and outputs involved.

A detailed decision tree(covering the process from fitting the PO model to obtaining and interpreting the PPO results) should be summerized

Official package example should be used if provided.

The research targets incude:

1. R `ordinal`
2. R `VGAM`
3. Stata `gologit2`
4. SAS `PROC LOGISTIC`

After the individual workflows are documented, an additional summary should compare the differences among these implementations in detail.

## Step 2 External Reference

A public dataset, **ESS6 United Kingdom**, should be used as a common external reference across all research targets.

For each software implementation:

1. The same dataset should be used.
2. The analysis code should be documented.
3. The main model outputs and results should be recorded.
4. The results should be reproducible.

The detailed analysis protocol, including preprocessing, variable selection, model specification, weighting, and comparison criteria, will be defined separately before the formal reference experiments begin.

## Step 3 PPO library design

PPO's basic workflow and detailed function should be designed in this step.


## Step 4 python library research

No mature and general-purpose PPO implementation has been identified in the Python ecosystem so far.

Existing Python libraries that support PO models should be investigated to determine how much of the designed workflow and functionality from Step 3 is already covered.

The remaining gaps should be clearly identified before development begins.


## Step 5 Implementation and Validation

Implement the PPO library according to the design established in Step 3.

The implementation should then be tested and validated against the external reference results established in Step 2.
