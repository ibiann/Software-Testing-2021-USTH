# Further suppose that test set T1 satisfies C1 on program P and test set T2 satisfies C2, also on P.

(a) Does T1 necessarily satisfy C2? Explain.

(b) Does T2 necessarily satisfy C1? Explain.

(c) If P contains a fault, and T2 reveals the fault, T1 does not
necessarily also reveal the fault. Explain.

# Answer:
A: Yes. T1 necessarily satisfy C2 as this follows directly from 
the definition of subsumption.

B: No. There is no reason to expect test requirements generated 
by C1 to be satisfied by T2.

C: No. it's not true. This is a difficult question to answer. Testers frequently believe that test sets for strong criteria are just as good as test sets for weaker criteria at detecting flaws. Subsumption, on the other hand, is about criteria, not test sets. There is no necessity that test set T2 be a subset of test set T1 in particular. As a result, it's possible that T2 contains the one test that reveals the flaw but T1 does not.
