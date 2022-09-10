# preact-render-to-string

## 5.2.3

### Patch Changes

- [#232](https://github.com/preactjs/preact-render-to-string/pull/232) [`2d5ca74`](https://github.com/preactjs/preact-render-to-string/commit/2d5ca74646f2f9f2e9ddeb20ed9c3fc47171c264) Thanks [@JoviDeCroock](https://github.com/JoviDeCroock)! - Performance enhancements

* [#238](https://github.com/preactjs/preact-render-to-string/pull/238) [`7cdf4d6`](https://github.com/preactjs/preact-render-to-string/commit/7cdf4d67abba622124902e53e016affbbebc647e) Thanks [@developit](https://github.com/developit)! - Fix the order of invocation for the "before diff" (`__b`) and "diffed" [options hooks](https://preactjs.com/guide/v10/options/).

## 5.2.2

### Patch Changes

- [#235](https://github.com/preactjs/preact-render-to-string/pull/235) [`2f6d6e8`](https://github.com/preactjs/preact-render-to-string/commit/2f6d6e8dd0573eb075273c2c9a20d7df289dacc8) Thanks [@marvinhagemeister](https://github.com/marvinhagemeister)! - Remove duplicate type path in `package.json`. Only one of `types` or `typings` is needed.

* [#228](https://github.com/preactjs/preact-render-to-string/pull/228) [`e4fe799`](https://github.com/preactjs/preact-render-to-string/commit/e4fe7992d717eb3cb8740d2d28696bf2ba6c3d1e) Thanks [@developit](https://github.com/developit)! - Improve string encoding performance by ~50%

- [#229](https://github.com/preactjs/preact-render-to-string/pull/229) [`d83def7`](https://github.com/preactjs/preact-render-to-string/commit/d83def7c1765c4ad1665598905531f5157366abd) Thanks [@JoviDeCroock](https://github.com/JoviDeCroock)! - Split up hot paths and make separate path for opts.pretty

## 5.2.1

### Patch Changes

- [#224](https://github.com/preactjs/preact-render-to-string/pull/224) [`645f3cb`](https://github.com/preactjs/preact-render-to-string/commit/645f3cb0d5364bcf945cb498e44dcbd381183c90) Thanks [@rschristian](https://github.com/rschristian)! - Ensures `defaultChecked` is serialized as `checked` attribute

* [#225](https://github.com/preactjs/preact-render-to-string/pull/225) [`31ac323`](https://github.com/preactjs/preact-render-to-string/commit/31ac32332c49876b84f73beb1e0732e76283cc5f) Thanks [@JoviDeCroock](https://github.com/JoviDeCroock)! - Optimize perf by using smarter string builder

## 5.2.0

### Minor Changes

- [#219](https://github.com/preactjs/preact-render-to-string/pull/219) [`250c15f`](https://github.com/preactjs/preact-render-to-string/commit/250c15fbc01e28c3934689e2a846e441709d829f) Thanks [@developit](https://github.com/developit)! - Implement hook state settling. Setting hook state during the execution of a function component (eg: in `useMemo`) will now re-render the component and use the final result. Previously, these updates were dropped.

## 5.1.21

### Patch Changes

- [#215](https://github.com/preactjs/preact-render-to-string/pull/215) [`a8672db`](https://github.com/preactjs/preact-render-to-string/commit/a8672db2be9eb96f29d778d1fcea58d00cb5ce44) Thanks [@AleksandrHovhannisyan](https://github.com/AleksandrHovhannisyan)! - Don't add selected attribute to <option> elements if they already contain that attribute

## 5.1.20

### Patch Changes

- [#209](https://github.com/preactjs/preact-render-to-string/pull/209) [`298d05e`](https://github.com/preactjs/preact-render-to-string/commit/298d05e5a29620ee9865b4cdb14c28464eebbd47) Thanks [@rschristian](https://github.com/rschristian)! - On empty className w/ compat, class attribute will no longer be duplicated

* [#205](https://github.com/preactjs/preact-render-to-string/pull/205) [`6d47c5a`](https://github.com/preactjs/preact-render-to-string/commit/6d47c5ae3821a11232d865687e97b1d37faa955f) Thanks [@JoviDeCroock](https://github.com/JoviDeCroock)! - Fix serialize defaultValue as value attribute