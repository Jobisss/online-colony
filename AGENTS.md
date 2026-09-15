# Project instructions

## Graph traceability

After changing project documentation or cross-system decisions, update the impact graph with:

```text
/graphify E:\jobisss\online-colony --update
```

Use the generated graph to review all connected policies, interactions, systems, and source sections before considering a transversal change complete.

For every transversal change, also perform a consistency audit:

- compare the new decision against connected documents and flag contradictory rules;
- check for conflicts between resolved and open decisions;
- review new cross-community connections and `AMBIGUOUS` relations as possible design insights;
- report the affected files, the contradiction (if any), and the new connection before closing the change.
