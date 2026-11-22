# Tech standards
- TypeScript strict mode, React + Vite, Vitest, fast-check.
- No backend. The simulation engine runs in the browser.
- Engine code must be deterministic: never use Date.now() or
  Math.random() inside src/engine. Use the virtual clock and the
  seeded PRNG only.
- Same seed + same scenario must give an identical event trace.
- Every engine module needs unit tests; invariants need
  property-based tests.
- Never claim support the code does not demonstrate.