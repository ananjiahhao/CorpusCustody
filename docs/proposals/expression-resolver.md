# Proposal: SPDX expression resolver

Status: closed, not planned for this iteration.

Supporting OR and WITH expressions fully would need a small resolver with
operator precedence, plus a decision table for what a satisfying choice looks
like per consumer. For now the gate classifies the expression conservatively
and reports it for review. A future parser can replace the classifier without
changing the report contract.
