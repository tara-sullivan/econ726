For lecture 1:
- [ ] Add math that shows why observed differences in outcomes equals causal effects + selection bias

For lecture 6 (slides-06-matching-propensity.tex):
Check against Taddy, Business Data Science ch. 6:
- [ ] A6: Structural model conditions written as `\epsilon \vert D, X = 0` and `v \vert X = 0` (LTE slides + "LTE and propensity score matching"). Should these be E[eps | D, X] = 0 and E[v | X] = 0?
- [ ] A7: "Estimation of LTE" slide says psi is the treatment effect of D on Y. Check whether it should be gamma (psi is the coefficient on D-hat).
- [ ] A8: "LTE and propensity score matching" item 2: `\hat{p(X)}` should be `\hat{p}(X)`; also check the formula E[Y / p-hat(X) | D] = alpha + D gamma against the book (doesn't match the IPW estimator derived earlier).
Discuss:
- [x] B (resolved: cut proof slide 1; relabeled slide 2 as balancing property; cited R&R 1983 / MHE for theorem; added testability bullet to DAG slide): Propensity score theorem proof. Slide 1 sets up E[D | Y(j), p(X)] but slide 2 proves E[D | X, p(X)] = E[D | p(X)] (balancing property), never using Y(j) or CIA. Compare to MHE proof. Also `&=` vs `=&` alignment mix in the slide-2 align*.
Hold:
- [x] D1: Title "Linear regression + Matching" and Housekeeping slide (finish linear regression; empty homework bullet) look stale from lecture 5.
- [ ] D2: "Unconditional ATE" slide reverts to binary sum over x in {0,1} after generalizing to vector X.
- [ ] D3: delta_ATE written with potential outcomes, whereas delta_X elsewhere uses observed Y_i (MHE uses observed Y_i).
- [ ] D4: Binary slides switch between delta_0/delta_1 and delta_{X_i=0}/delta_{X_i=1}.
- [ ] D5: Propensity Score Theorem slide: "to achieve CIA" -> maybe "to eliminate selection bias".
- [ ] E: Overfull hboxes near selection-bias align (Motivating example), the delta table slide, and Fact #2 (cont.).
- [x] Reorder: "Unconditional Average Treatment Effect" and the two "Matching and regression" slides feel out of place after the new subclassification/curse/exact/nearest-neighbor frames. Move them.
- [ ] Exact matching: mention how to estimate the ATE (Mixtape eq. 5.27, sign term (2D_i - 1)) and its limitations (needs matches for untreated units too; fails in the job training example, e.g. comparison unit 29 is age 51 and no trainee is).
