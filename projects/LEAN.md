---
layout: project
type: project
image: img/lean.png
title: "Coding Proofs in LEAN"
date: 2025
published: true
labels:
  - LEAN V4
  - Mathematical Proofs
  - JLA
summary: "Under Professor Kjos-Hansen I usedLEAN V4 and Mathlib to code mathematical proofs from the Journal of Logic and Analysis, to be added as formal marginalia for an article published in Marginis."
---
I worked on formalizing mathematical proofs from the *Journal of Logic and Analysis* using LEAN V4 and Mathlib. My job was to take the proofs from the journal and translate them into a form that LEAN could check, making sure that every step was completely correct and could logically compile. By doing this, I was able to create fully verified versions of these proofs, which could then be used as reliable references for other mathematicians.

I worked closely with Professor Kjos Hansen on this project, who helped guide me through both the technical and theoretical parts of using LEAN. My work ended up being added as formal marginalia for an article published in *Marginis* on the UH Manoa Math Website. Overall, this experience gave me a lot of practice in formal proof writing and showed me how computational tools like LEAN can be applied to real research in logic and analysis.
 
For example the code below shows lemmas created in order to prove (by automation) the density of the rationals in the reals, and then more elaborately the density of the rationals Q in [0,1].

```lean
lemma real_dense : "∀x::real. ∀y::real. (x < y ⟶ (∃z::real. x < z ∧ z < y))"
  using dense by blast

lemma rat_dense_in_real : "∀x::real. ∀y::real. (x < y ⟶ (∃z::rat. x < real_of_rat(z) ∧ real_of_rat(z) < y))"
  by (simp add: of_rat_dense)

lemma rat_dense_in_real_unit : "∀x::real. ∀y::real. (
  (x < y ∧  (0 ≤ x ∧ x ≤ 1) ∧  (0 ≤ y ∧ y ≤ 1))  ⟶
  (∃z::rat.(0 ≤ real_of_rat(z) ∧ real_of_rat(z) ≤ 1) ∧ x < real_of_rat(z) ∧ real_of_rat(z) < y)
)"
```

You can learn more at the [UH Manoa Math Marginis Website!](https://math.hawaii.edu/wordpress/marginis/jla/).
