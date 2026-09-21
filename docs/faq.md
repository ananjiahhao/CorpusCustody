# FAQ

**Does CorpusCustody replace legal review?**
No. It replaces manual license triage: it classifies, computes obligations,
and records provenance. A human still decides what is acceptable.

**What does the gate do with an unknown license?**
It blocks the record and names the field that produced the unknown class, so
classification can start from the exact value.

**Why is the report deterministic?**
So two runs over the same manifest are byte identical and a diff shows only
what changed in the corpus.
