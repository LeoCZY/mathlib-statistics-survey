# A summary level markdown


## where are varaibles name and theorems name living?
here is an exmaple:

 ```lean
 import Mathlib

namespace ProbabilityTheory

variable {Ω : Type*}

section Cond

variable {s : Set Ω}

def keep (x : Ω) : Ω := x

theorem mem_self (x : Ω) (hx : x ∈ s) : x ∈ s :=
  hx

-- Ω, s, keep, and mem_self can all be used directly here.

end Cond

-- Ω is still in scope.
-- s is no longer in scope.
-- keep and mem_self can still be used directly
-- because we are still inside the ProbabilityTheory namespace.

#check keep
#check mem_self
#check sameRay_iff_of_norm_eq

end ProbabilityTheory

-- Ω is no longer in scope.
-- keep and mem_self still exist,
-- but they must now be referenced by their fully qualified names.

#check ProbabilityTheory.keep
#check ProbabilityTheory.mem_self
 ```



reference:
https://lean-lang.org/theorem_proving_in_lean4/Dependent-Type-Theory/#variables-and-sections
