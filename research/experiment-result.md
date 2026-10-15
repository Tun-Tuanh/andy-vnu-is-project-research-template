# Experimental Results & Empirical Analysis

> [!NOTE]
> **Instructions:**
> Use this document to compile, visualize, and discuss the quantitative and qualitative outcomes of the experiments defined in [`research/experiment-design.md`](file:///f:/thinkprompt/code/researches/project-research-template/research/experiment-design.md).

---

## 1. Primary Benchmark Results

The table below summarizes performance across baselines and the proposed system across all evaluation metrics. Values are reported as `Mean ± Std` across multiple runs (`N=3` seeds: `42`, `1337`, `2026`).

| Model / System | Primary Metric: `[e.g., F1 / Acc] (% ↑)` | Secondary Metric: `[e.g., Precision] (% ↑)` | Latency `(ms/sample ↓)` | Model Size `(# Params)` | Stat. Sig. `(p-value vs B4)` |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **B1: Heuristic Baseline** | `00.0 ± 0.0` | `00.0 ± 0.0` | `0.5 ms` | `0` | - |
| **B2: Classical ML (XGBoost)** | `00.0 ± 0.0` | `00.0 ± 0.0` | `2.1 ms` | `~500K` | `p < 0.001` |
| **B3: Standard SOTA (RoBERTa / ResNet)** | `00.0 ± 0.0` | `00.0 ± 0.0` | `14.2 ms` | `125M` | `p = 0.018` |
| **B4: Competitive SOTA Baseline** | `00.0 ± 0.0` | `00.0 ± 0.0` | `18.6 ms` | `140M` | Reference |
| **Ours: Full Proposed Method** | **`00.0 ± 0.0`** | **`00.0 ± 0.0`** | **`00.0 ms`** | **`XX M`** | **`p = 0.003*`** |

*Note: Statistical significance evaluated using a two-tailed paired t-test ($\alpha = 0.05$).*

---

## 2. Ablation Study Results

To assess the individual impact of each design choice, we perform systematic component ablations:

| Variant | Configuration | Primary Metric `(% ↑)` | $\Delta$ vs Full Model | Key Takeaway |
| :--- | :--- | :---: | :---: | :--- |
| **Full Model** | All proposed components | **`00.0 ± 0.0`** | - | Complete proposed pipeline |
| **w/o Component A** | Ablate `[e.g., Attention Layer]` | `00.0 ± 0.0` | `- X.X%` | Demonstrates necessity of Component A |
| **w/o Component B** | Ablate `[e.g., Data Augmentation]` | `00.0 ± 0.0` | `- Y.Y%` | Validates contribution of Component B |
| **w/ Standard Loss** | Replace custom loss with CrossEntropy | `00.0 ± 0.0` | `- Z.Z%` | Proves efficacy of proposed objective function |

---

## 3. Visualizations & Performance Curves

> Save generated evaluation charts into `research/experiment-result/figures/` and link them here.

### 3.1 Convergence & Training Dynamics
*`![Training & Validation Loss Convergence](research/experiment-result/figures/loss_curve.png)`*
- **Observation:** `[Describe convergence speed, presence of overfitting, stability across epochs]`

### 3.2 Performance Comparison Across Data Subsets
*`![F1 Score by Category / Class](research/experiment-result/figures/category_breakdown.png)`*
- **Observation:** `[Highlight which specific classes or edge cases showed greatest improvement]`

---

## 4. Discussion & Error Analysis

### 4.1 Why Does the Proposed Method Outperform Baselines?
- `[Provide theoretical and empirical rationale for observed performance improvements]`
- `[Connect back to the hypotheses stated in research-methodology.md]`

### 4.2 Failure Mode & Error Analysis
Analyze 3–5 representative failure cases where the model failed or produced erroneous outputs:

| Case ID | Input / Context | Ground Truth | Model Prediction | Root Cause Analysis |
| :-: | :--- | :--- | :--- | :--- |
| **E1** | `[Brief description of input]` | `[True Class]` | `[Predicted Class]` | `[e.g., High lexical ambiguity / out-of-vocabulary terms]` |
| **E2** | `[Brief description of input]` | `[True Class]` | `[Predicted Class]` | `[e.g., Insufficient training examples for minority class]` |
| **E3** | `[Brief description of input]` | `[True Class]` | `[Predicted Class]` | `[e.g., Noise in input sensors or labels]` |

---

## 5. Answers to Research Questions

- **RQ1 Answer:** `[Summarize empirical conclusion based on EXP-01 through EXP-03 results]`
- **RQ2 Answer:** `[Summarize empirical conclusion based on ablation study EXP-04 and EXP-05]`
- **RQ3 Answer:** `[Summarize empirical conclusion on efficiency and latency trade-offs]`
