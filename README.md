# Logic and sets notes
Study material for logic and sets University
- [A Crash Course in Formal Logic](https://www.youtube.com/watch?v=ywKZgjpMBUU)
- [Sentence Semantics](https://www.youtube.com/watch?v=XLvv_5meRNM&list=PLRIMXVU7SGRJF8gxD70oZPBoFAYxGs4QL&index=5)
- [Introduction to predicate logic](https://www.youtube.com/channel/UCmVAIqvL7852sE23K5D1ldg)

## Midterm material
### Sheffer stroke:
- [Discrete Mathematics](Sheffer Stroke Examples](https://www.youtube.com/watch?v=vIWyeblTuwk)

### Island of truth tellers and liars 
- [pdf](https://sheilamorr.weebly.com/uploads/5/6/8/0/5680346/frederixon_cs1_articlefortask.pdf)


### XOR
- ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/79e6102bc63d3111d3acd7439f03d86ceee76c05)
- ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/f8dfc84698010baba9bdd1f4b796295e9829079f)






## Final 


### Semantic entailments
Alpha is entailed by beta iff Alpha ^ not-Beta is unsatisfiable
#### How to check it manually:
- draw the truth table 
- Look for the T
- for each T on the right side must have a T on the left side. 
- if not the semantic entailement is not valid.
- [Source 1](https://www.youtube.com/watch?v=IFO0E-4dbVU) 

### find, and deduce your CNF and DNF.
If you want to find DNF, you have to look at all rows that ends with T. When you find those rows, take the x,y, and z values from each respective column.
#### DNF: 
- Thus, you get (x∧y∧z)∨(x∧¬y∧¬z)∨(¬x∧y∧¬z)∨(¬x∧¬y∧z).
#### CNF
- Similarly, you can find CNF you negate each value in the following way(¬x∨¬y∨z)∧(¬x∨y∨¬z)∧(x∨¬y∨¬z)∧(x∨y∨z).
- [Propositional Normal Forms](http://swtv.kaist.ac.kr/courses/cs402-07/prop_logic4.pdf)
### CNF Algorithm Satisfiability
- 1 - remove implication: (P∧Q)→Q, which becomes ¬(P∧Q)∨Q.
- 2 - remove double negations
- 3 - distribute the terms 
- 4 - check if it is in CNF  (_ or _) and ( _ or _) and ( _ or _)

### DPLL
- [Page 15-16](http://profs.sci.univr.it/~farinelli/courses/ar/slides/DPLL.pdf)

### OBDDs
- [Reduced ordered binary decision diagram](https://www.slideshare.net/RajeshYadav49/reduced-ordered-binary-decision-diagram-devi)
#### Rules:
- Rule C1: Collapse identical leaves.
- Rule C2: Eliminate superfluous non-leaves.
- Rule C3: Remove duplicate non-leaves.
