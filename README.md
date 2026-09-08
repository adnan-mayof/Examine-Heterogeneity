# Step 16 — Examine Heterogeneity
[← Previous Step: Conduct the Meta-Analysis](https://github.com/adnan-mayof/Conduct-the-Meta-Analysis/blob/main/README.md)

## Maya’s Evidence Synthesis Journey

### Why Are the Study Results Different?

Maya has just completed her meta-analysis.

She started with **111 eligible studies** for her systematic review.

After assessing the available quantitative information, **22 studies** contributed to the planned meta-analysis.

In Step 14, she calculated the effect sizes.

In Step 15, she statistically combined those effects.

For this illustrative example, Maya obtained:

> **Pooled Hedges' g = 0.64 (95% CI [0.52, 0.76])**

Maya is excited.

> **Maya:** “We have the overall effect!”

Her mentor looks at the forest plot.

> **Mentor:** “Yes. But look at the individual studies.”

Maya looks more closely.

Some studies have effects around **0.40**.

Others are around **0.60**.

Some are close to **0.80**.

> **Maya:** “The effects are different.”

> **Mentor:** “Exactly.”

> **Maya:** “But isn't that normal?”

> **Mentor:** “It can be. The important question is: **how much do the effects differ, and what might explain that variation?**”

Maya realizes that getting a pooled effect is not the end of the analysis.

---

# 1. What Is Heterogeneity?

**Heterogeneity** refers to variation among the effect estimates from different studies.

For example:

| Study | Hedges' g |
| ----- | --------: |
| S001  |      0.62 |
| S002  |      0.60 |
| S003  |      0.63 |
| S004  |      0.80 |
| S005  |      0.57 |
| S006  |      0.71 |
| S007  |      0.45 |
| S008  |      0.83 |

The effect sizes are not identical.

Maya now asks:

> **“Are these differences simply due to sampling variation, or do the studies have genuinely different underlying effects?”**

That is the central question of heterogeneity assessment.

---

# 2. Why Would Study Effects Differ?

Maya's review examines AI-powered learning technologies.

But the studies are not identical.

They may differ in:

* students
* educational levels
* AI technologies
* AI functions
* intervention duration
* instructional approaches
* comparison groups
* learning environments
* outcome measures
* study designs

For example:

| Study | AI Technology | Students      | Duration | Outcome     |
| ----- | ------------- | ------------- | -------- | ----------- |
| S001  | AI tutor      | Undergraduate | 8 weeks  | Achievement |
| S002  | Chatbot       | Undergraduate | 4 weeks  | Knowledge   |
| S003  | Adaptive AI   | High school   | 12 weeks | Achievement |
| S004  | Generative AI | University    | 6 weeks  | Skill       |

Maya realizes:

> **Maya:** “So the studies are estimating effects under different conditions.”

> **Mentor:** “Exactly. That is one reason we need to examine heterogeneity.”

---

# 3. Sampling Variation and Heterogeneity

Maya's mentor draws two sources of variation.

```text
Differences among observed effect sizes
                 │
        ┌────────┴────────┐
        ↓                 ↓
Sampling variation   Between-study
                     heterogeneity
```

### Sampling variation

Each study estimates an effect using a sample rather than the entire population.

Therefore, study estimates naturally vary.

### Between-study heterogeneity

The underlying effects themselves may differ across studies.

For example, an AI intervention may work differently:

* with different learners
* in different settings
* for different outcomes
* at different intervention durations

Maya needs statistical methods to investigate the amount of variation.

---

# 4. Three Important Heterogeneity Statistics

Maya's mentor introduces three statistics:

1. **Cochran's Q**
2. **I²**
3. **τ² (tau-squared)**

They are related, but they do not mean the same thing.

| Statistic | What it tells Maya                                                                            |
| --------- | --------------------------------------------------------------------------------------------- |
| Q         | Whether observed variation is greater than expected from sampling error alone under the model |
| I²        | The relative proportion of observed variability attributed to between-study heterogeneity     |
| τ²        | The estimated variance of the underlying true effects                                         |

Maya writes them down.

> **Maya:** “So I should report all three?”

> **Mentor:** “They can provide complementary information, but always interpret them in the context of your model and data.”

---

# 5. Cochran's Q

The first statistic Maya examines is **Cochran's Q**.

Q evaluates whether the observed differences among study effects are greater than would be expected from sampling error alone under the assumed model.

Conceptually:

> **Q asks:**
> “Is there more variation among the observed effects than we would expect from sampling error alone?”

A larger Q relative to its degrees of freedom can provide evidence of heterogeneity.

---

# 6. Maya's Q Result

Suppose Maya obtains:

> **Q(21) = 48.6, p < .001**

Maya asks:

> **Maya:** “So there is heterogeneity?”

> **Mentor:** “The Q test provides evidence that the observed variation is greater than would be expected from sampling error alone under the model.”

But the mentor adds:

> **Mentor:** “Don't rely on Q alone.”

The Q statistic is influenced by the number of studies.

With relatively few studies, the test may have limited ability to detect heterogeneity.

With many studies, even relatively modest heterogeneity can produce a statistically significant result.

Therefore, Maya should examine other heterogeneity statistics too.

---

# 7. I²

Next, Maya examines **I²**.

I² describes the proportion of observed variability in the effect estimates that is attributed to between-study heterogeneity rather than sampling error, under the assumptions of the model.

Conceptually:

```text
Observed variability
        │
        ├── Sampling variation
        │
        └── Between-study heterogeneity
```

I² focuses on the **relative contribution** of between-study heterogeneity.

---

# 8. Maya's I² Result

Suppose Maya obtains:

> **I² = 58%**

Maya asks:

> **Maya:** “Does that mean 58% of the studies are different?”

> **Mentor:** “No.”

I² is **not the percentage of studies with different effects**.

It is a measure of the proportion of observed variability attributed to between-study heterogeneity.

This distinction is important.

---

# 9. Common Descriptive I² Values

Maya encounters commonly used descriptive conventions:

|  I² | Common descriptive label                            |
| --: | --------------------------------------------------- |
|  0% | No observed heterogeneity beyond sampling variation |
| 25% | Low                                                 |
| 50% | Moderate                                            |
| 75% | High                                                |

Her mentor immediately adds:

> **Mentor:** “These are conventions, not universal rules.”

The interpretation of I² depends on:

* the research context
* the outcome
* study precision
* effect-size metric
* magnitude of effects
* assumptions of the analysis

Therefore, Maya should not use an I² threshold as an automatic decision rule.

---

# 10. τ² — Tau-Squared

Maya asks:

> **Maya:** “What does tau-squared tell me?”

Her mentor explains:

> **Mentor:** “τ² estimates the variance of the underlying true effects across studies in a random-effects model.”

Maya compares the statistics.

### I²

Relative measure of heterogeneity.

### τ²

Estimated variance of the underlying true effects.

She writes:

> **I² → relative heterogeneity**

> **τ² → between-study variance**

---

# 11. Why Does τ² Depend on the Effect-Size Metric?

Maya asks:

> **Maya:** “Can I compare tau-squared directly across any meta-analysis?”

> **Mentor:** “Not without considering the effect-size scale.”

τ² is expressed on the squared scale of the effect-size metric.

For example, if Maya uses Hedges' g, τ² is based on the corresponding standardized effect-size scale.

Therefore, τ² needs to be interpreted in relation to the effect-size metric.

---

# 12. Maya's Heterogeneity Results

For the illustrative dataset, suppose Maya obtains:

| Statistic | Result |
| --------- | -----: |
| Q         |   48.6 |
| df        |     21 |
| p-value   | < .001 |
| I²        |    58% |
| τ²        |  0.052 |

Maya summarizes:

> “There is evidence of between-study heterogeneity. I² is 58%, and the estimated τ² is 0.052.”

Her mentor responds:

> **Mentor:** “Good. Now we need to understand what that means for interpretation.”

---

# 13. Heterogeneity Is Not Automatically a Problem

Maya asks:

> **Maya:** “Does heterogeneity mean something went wrong?”

> **Mentor:** “Not necessarily.”

In many evidence-synthesis projects, researchers expect effects to vary.

For Maya's AI-learning review, different effects may be scientifically reasonable.

An AI tutor might produce a different effect from:

* an AI writing assistant
* an automated feedback system
* a conversational chatbot
* an adaptive learning system

Likewise, effects may differ by:

* student population
* learning context
* duration
* outcome

Heterogeneity can therefore be **informative**.

---

# 14. Why Does Heterogeneity Matter?

Suppose the studies produce:

| Study | Effect |
| ----- | -----: |
| S001  |   0.10 |
| S002  |   0.25 |
| S003  |   0.50 |
| S004  |   0.80 |
| S005  |   1.10 |

Maya could calculate an overall effect.

But she should also ask:

> **“Why are some effects small while others are large?”**

The pooled effect may provide a useful overall summary while still hiding meaningful variation.

That is why heterogeneity is important.

---

# 15. Returning to the Forest Plot

Maya opens her forest plot again.

She can visually inspect:

* the direction of effects
* the magnitude of effects
* the precision of each estimate
* the spread of the estimates
* the pooled estimate

For example:

```text id="z7bq9k"
                 Effect
          -1      0      1      2

S001              ◆───
S002                ◆──
S003              ◆────
S004                   ◆────
S005              ◆──
S006                 ◆───
S007          ◆────
S008                    ◆──

                  ◇
             Pooled Effect
```

The forest plot helps Maya see that the effects are not identical.

However:

> **A forest plot should not be the only basis for judging heterogeneity.**

Statistical measures provide additional information.

---

# 16. What If Heterogeneity Is High?

Maya asks:

> **Maya:** “Suppose I² is very high. Should I stop the meta-analysis?”

> **Mentor:** “Not automatically.”

A high heterogeneity estimate does not by itself mean that the meta-analysis should be abandoned.

Maya should consider:

* whether the studies are conceptually comparable
* whether the research question supports synthesis
* whether the effect-size metric is appropriate
* whether study differences are expected
* whether the statistical model is appropriate
* whether potential sources of variation can be investigated

The goal is not simply to eliminate heterogeneity.

The goal is to **understand and appropriately model it**.

---

# 17. Don't Use I² as a Simple Go/No-Go Rule

Maya writes:

> **I² > 50% ≠ automatically stop**

> **I² > 75% ≠ automatically stop**

The decision should not be based on a single threshold.

For example, two meta-analyses could both have:

**I² = 60%**

But the substantive meaning could be very different depending on:

* outcome
* population
* intervention
* measurement
* study design
* research question

Therefore, interpretation requires context.

---

# 18. Random-Effects Models and Heterogeneity

Maya remembers that she used a random-effects model in Step 15.

She asks:

> **Maya:** “Does the random-effects model solve the heterogeneity problem?”

> **Mentor:** “No. It models between-study variation.”

A random-effects model assumes that the true effects can vary across studies.

It incorporates an estimate of between-study variance into the model.

It does **not** make the studies identical.

It does **not** remove heterogeneity.

It does **not** explain why effects differ.

---

# 19. Prediction Interval

Maya's mentor introduces one more useful concept.

> **Mentor:** “Because you're using a random-effects model, you can also consider a prediction interval.”

A **prediction interval** can help communicate the range of effects that might reasonably be expected in a future comparable study, taking estimated between-study heterogeneity into account.

Suppose Maya obtains:

> **Pooled Hedges' g = 0.64**

> **95% CI [0.52, 0.76]**

and:

> **95% Prediction Interval [0.18, 1.10]**

Maya notices that the prediction interval is wider.

> **Maya:** “So the average effect is estimated fairly precisely, but a future study could have a substantially different effect.”

> **Mentor:** “Exactly.”

---

# 20. Confidence Interval vs. Prediction Interval

| Interval            | Main question                                                         |
| ------------------- | --------------------------------------------------------------------- |
| Confidence interval | How uncertain is the estimated average effect?                        |
| Prediction interval | What range of effects might be expected in a future comparable study? |

This distinction helps Maya communicate both:

**the average effect**

and

**the variation that may occur across settings or future studies.**

---

# 21. What Heterogeneity Statistics Cannot Tell Maya

Maya now understands an important limitation.

Suppose:

> **I² = 58%**

This tells her something about variation.

But it does **not** tell her:

* which AI technology caused the variation
* whether intervention duration explains it
* whether learner level explains it
* whether study design explains it
* whether outcome type explains it

Heterogeneity statistics describe variation.

They do not automatically explain its source.

---

# 22. Looking Back at the Extraction Dataset

Maya returns to the data she prepared in Step 13.

She already collected variables such as:

| Variable              | Example       |
| --------------------- | ------------- |
| AI technology         | AI tutor      |
| AI function           | Feedback      |
| Learner level         | Undergraduate |
| Intervention duration | 8 weeks       |
| Outcome               | Achievement   |
| Study design          | RCT           |
| Learning context      | University    |

Maya realizes that these variables may help explain differences among effect sizes.

---

# 23. From Heterogeneity to Moderators

Maya asks:

> **Maya:** “Can I test whether these characteristics explain the differences?”

> **Mentor:** “Yes. That's the next stage.”

For example:

### Moderator question

> “Do intervention durations of different lengths produce different effect estimates?”

Or:

> “Do different AI functions produce different effect estimates?”

Or:

> “Do effects differ between undergraduate and high-school learners?”

This leads directly to **moderator analysis**.

---

# 24. Heterogeneity vs. Moderator Analysis

Maya writes the distinction in her notebook.

### Heterogeneity asks:

> **“How much do the effects differ?”**

### Moderator analysis asks:

> **“Are study characteristics associated with differences in effects?”**

For example:

```text id="c1k1q5"
Study effects differ
        ↓
Heterogeneity
        ↓
Potential explanations
        ↓
Study characteristics
        ↓
Moderator analysis
```

---

# 25. Maya's Heterogeneity Workflow

Maya creates a workflow for her project.

```text id="m8t4qz"
Individual effect sizes
        ↓
Meta-analysis
        ↓
Pooled effect
        ↓
Forest plot
        ↓
Examine Q
        ↓
Estimate I²
        ↓
Estimate τ²
        ↓
Consider prediction interval
        ↓
Interpret variation in context
        ↓
Identify plausible explanations
        ↓
Step 17: Examine Moderators
```

---

# 26. Example Write-Up

For the illustrative dataset, Maya might report:

> **Twenty-two studies contributed to the primary meta-analysis. A random-effects model estimated a pooled Hedges' g of 0.64 (95% CI [0.52, 0.76]). There was evidence of between-study heterogeneity, Q(21) = 48.6, p < .001, with I² = 58% and τ² = 0.052.**

If a prediction interval was calculated, Maya could also report it.

For example:

> **The 95% prediction interval ranged from 0.18 to 1.10, indicating that effects in future comparable studies may vary substantially around the estimated average effect.**

These values are **illustrative** and should be replaced by the actual results of the analysis.

---

# 27. What Maya Should Avoid

Maya creates a checklist.

### Avoid:

* Saying I² is the percentage of studies that differ.
* Treating I² as an automatic decision rule.
* Assuming high heterogeneity automatically invalidates the meta-analysis.
* Treating Q as a measure of the size of heterogeneity.
* Interpreting τ² without considering the effect-size scale.
* Assuming the random-effects model eliminates heterogeneity.
* Assuming heterogeneity statistics identify its causes.
* Treating the pooled effect as the effect experienced by every study.
* Selecting moderators simply because they produce interesting results.

### Instead:

* Report the heterogeneity statistics.
* Interpret them in context.
* Consider the study characteristics.
* Follow the prespecified analysis plan.
* Investigate plausible sources of variation systematically.

---

# 28. What Happens to the 89 Studies?

Maya remembers that **89 eligible studies** did not contribute to the primary meta-analysis.

She asks:

> **Maya:** “Do those studies contribute to I² or τ²?”

> **Mentor:** “Not to this particular quantitative synthesis.”

The heterogeneity statistics are calculated from the effect estimates included in the relevant meta-analysis.

The 89 studies remain part of the systematic review.

They can still contribute to:

* narrative synthesis
* evidence tables
* descriptive findings
* contextual interpretation
* discussion
* identification of research gaps

---

# 29. Maya's Final Understanding

Maya now looks at the whole process.

```text id="z3f4ra"
111 eligible studies
        ↓
22 studies in quantitative synthesis
        ↓
Effect sizes
        ↓
Pooled effect
        ↓
How much do effects differ?
        ↓
Heterogeneity
        ↓
Why might effects differ?
        ↓
Moderators
```

She understands that the meta-analysis does not end when she obtains the pooled effect.

The pooled effect tells her:

> **“What is the estimated average effect?”**

Heterogeneity tells her:

> **“How much do the study effects vary?”**

The next step will ask:

> **“What might explain that variation?”**

---

# 30. Key Takeaways

By the end of Step 16, Maya understands:

1. Heterogeneity refers to variation among study effect estimates.
2. Differences among effect estimates can arise from sampling variation and genuine differences among underlying effects.
3. Studies in an evidence synthesis may differ in populations, interventions, contexts, outcomes, and methods.
4. Cochran's Q assesses whether observed variation is greater than expected from sampling error alone under the model.
5. I² describes the relative proportion of observed variability attributed to between-study heterogeneity.
6. I² is not the percentage of studies with different results.
7. τ² estimates the variance of the underlying true effects in a random-effects model.
8. Q, I², and τ² provide different information.
9. Common I² values such as 25%, 50%, and 75% are descriptive conventions, not universal decision rules.
10. Heterogeneity is not automatically a problem.
11. A high I² value does not automatically mean that the meta-analysis should be abandoned.
12. A random-effects model accommodates between-study variation; it does not eliminate or explain it.
13. A confidence interval around the pooled effect and a prediction interval answer different questions.
14. Heterogeneity statistics describe variation but do not automatically identify its causes.
15. Study characteristics may help explain heterogeneity through moderator analysis.
16. Only studies contributing effect estimates to a particular quantitative synthesis contribute to that synthesis's heterogeneity statistics.
17. The 89 studies not included in the primary meta-analysis remain part of the systematic review.
18. The next step is to examine whether prespecified study characteristics explain variation in the effects.

---

# Repository Structure

```text id="b8k2q1"
step-16-examine-heterogeneity/
│
├── README.md
│
├── heterogeneity/
│   ├── heterogeneity-guide.md
│   ├── q-statistic.md
│   ├── i2.md
│   ├── tau2.md
│   ├── prediction-interval.md
│   └── heterogeneity-results.md
│
├── data/
│   └── meta-analysis-data.xlsx
│
├── figures/
│   └── forest-plot.png
│
├── documentation/
│   ├── heterogeneity-decisions.md
│   └── analysis-log.md
│
└── assessment/
    └── assessment.md
```

---

# Assessment

## Instructions

Choose the best answer for each question.

### 1. What does heterogeneity refer to?

A. The number of databases searched
B. Variation among study effect estimates
C. The number of reviewers
D. The number of eligible studies

### 2. Why might effect sizes differ across studies?

A. Studies may differ in populations, interventions, contexts, outcomes, and methods
B. Effect sizes are always identical
C. Every study must have a different research question
D. Statistical analysis creates differences automatically

### 3. What does Cochran's Q evaluate?

A. Whether observed variation is greater than expected from sampling error alone under the model
B. The magnitude of the pooled effect
C. The number of participants
D. The risk of bias

### 4. What does I² describe?

A. The percentage of studies with positive findings
B. The percentage of participants in the intervention group
C. The proportion of observed variability attributed to between-study heterogeneity
D. The number of studies included in the meta-analysis

### 5. What does τ² estimate in a random-effects model?

A. The average sample size
B. The variance of underlying true effects across studies
C. The number of effect sizes
D. The p-value of the pooled effect

### 6. Maya obtains I² = 58%. What does this mean?

A. Exactly 58% of the studies have different results
B. 58% of participants benefited from the intervention
C. A substantial proportion of observed variability is attributed to between-study heterogeneity
D. The meta-analysis must be discontinued

### 7. Which statement about I² is most appropriate?

A. I² automatically determines whether studies can be combined
B. I² identifies the exact cause of heterogeneity
C. I² should be interpreted in the context of the research and analysis
D. I² represents the percentage of significant studies

### 8. Why should Maya not rely only on Cochran's Q?

A. Its behavior can depend on the number of studies
B. Q cannot be calculated in a meta-analysis
C. Q measures sample size
D. Q identifies moderators automatically

### 9. What does a random-effects model allow?

A. All studies to have identical underlying effects
B. Underlying effects to vary across studies
C. All heterogeneity to disappear
D. All studies to receive identical weights

### 10. What does a prediction interval provide?

A. The expected range of effects in a future comparable study, incorporating estimated between-study variation
B. The percentage of significant studies
C. The number of eligible studies
D. The risk-of-bias score

### 11. How does a prediction interval differ from a confidence interval around the pooled effect?

A. They always answer exactly the same question
B. A confidence interval describes uncertainty around the average effect, while a prediction interval addresses the expected range of effects in a future study
C. A prediction interval measures risk of bias
D. A confidence interval measures study duration

### 12. What should Maya do if heterogeneity is substantial?

A. Automatically abandon the meta-analysis
B. Automatically remove the study with the largest effect
C. Investigate and interpret the variation according to the research question and analysis plan
D. Change the effect-size direction

### 13. What can heterogeneity statistics tell Maya?

A. How much the study effects vary
B. Exactly which moderator caused the variation
C. Which study should be published
D. Which database is best

### 14. Which question is a moderator question?

A. “How much do the study effects vary?”
B. “Do intervention durations help explain differences in effect sizes?”
C. “How many databases were searched?”
D. “How many references were downloaded?”

### 15. Which could be a moderator in Maya's review?

A. AI technology type
B. Reference-manager file name
C. Database search number
D. File storage location

### 16. Which studies contribute to heterogeneity statistics for a particular meta-analysis?

A. All 111 studies
B. Only studies contributing effect estimates to that quantitative synthesis
C. Only studies with positive results
D. Only the most recent studies

### 17. What should Maya avoid?

A. Reporting Q, I², and τ²
B. Considering study characteristics
C. Treating an I² threshold as an automatic decision rule for conducting the meta-analysis
D. Inspecting the forest plot

### 18. What is the next step after examining heterogeneity?

A. Return to database searching
B. Repeat full-text screening
C. Examine moderators
D. Recalculate the research question

---

# Answer Key

| Question | Answer |
| -------- | ------ |
| 1        | B      |
| 2        | A      |
| 3        | A      |
| 4        | C      |
| 5        | B      |
| 6        | C      |
| 7        | C      |
| 8        | A      |
| 9        | B      |
| 10       | A      |
| 11       | B      |
| 12       | C      |
| 13       | A      |
| 14       | B      |
| 15       | A      |
| 16       | B      |
| 17       | C      |
| 18       | C      |

---

## 🚀 Maya's Journey Continues

Maya has now **completed the Examine Heterogeneity stage**.
The next challenge is to conduct the Examine Moderators.

She is now ready to move to:

### Next Step

### **[Step 17 — Examine Moderators](https://github.com/adnan-mayof/Examine-Moderators/blob/main/README.md)**

 
