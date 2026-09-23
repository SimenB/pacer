---
'@tanstack/pacer': patch
---

fix(async-debouncer, async-throttler): stop AsyncDebouncer dropping a call made while the previous execution is still running, resolve each caller with its own execution's result instead of a stale one, and keep `isExecuting` true until all overlapping executions settle
