# Project instructions

## Graph traceability

Graphify must be installed before any graph query or update. Verify with `python -c "import graphify"`; if unavailable, install it with `python -m pip install graphifyy` and verify again.

After changing project documentation or cross-system decisions, update the impact graph from the repository root:

```text
/graphify . --update
```

Run it from the repository root so the command works on any machine; do not hardcode a local path.

Use the generated graph to review all connected policies, interactions, systems, and source sections before considering a transversal change complete.

The generated `graphify-out/cache/` directory is local state and is not tracked in git.

For every transversal change, also perform a consistency audit:

- compare the new decision against connected documents and flag contradictory rules;
- check for conflicts between resolved and open decisions;
- review new cross-community connections and `AMBIGUOUS` relations as possible design insights;
- report the affected files, the contradiction (if any), and the new connection before closing the change.
