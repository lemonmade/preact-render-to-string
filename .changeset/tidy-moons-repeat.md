---
'preact-render-to-string': patch
---

Render suspended subtrees in tree order in `renderToStringAsync`, so `useId()` produces the same values the client computes when it hydrates. Previously the renderer walked past a boundary, rendered the siblings that followed it, and only came back once the promise settled — and `useId()`, whose counter advances in render order, numbered everything inside the boundary differently than the client does.
