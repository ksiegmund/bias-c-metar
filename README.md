# Bias correction with meta-regression

This simulation examines how failure to adjust for a binary confounder changes
the estimated association between exposure and disease. Each point summarizes
the mean log odds ratio across 100 simulated populations. Colors represent the
confounder's conditional odds ratio ($OR_C$), while the horizontal axis shows
its population prevalence ($p_C$).

The solid lines are estimates from the adjusted model, `D ~ E + C`, and remain
near the true exposure effect, $\log(OR_E) = \log(4)$. The dotted lines are
estimates from the unadjusted model, `D ~ E`. Their increasing downward bias
shows how stronger or more prevalent confounding can mask—and eventually
reverse—the estimated exposure association when the confounder occurs only
among unexposed individuals.

![Mean adjusted and unadjusted log odds ratios across confounder prevalences and effect sizes](figures/mean-log-odds-ratios.png)
