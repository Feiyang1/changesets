# @changesets/apply-release-plan

## 3.0.2

### Patch Changes

- [`8fe77b6`](https://github.com/atlassian/changesets/commit/8fe77b614b726b861900e69c015c8876f64ed04f) [#366](https://github.com/atlassian/changesets/pull/366) Thanks [@Blasz](https://github.com/Blasz)! - Fix release version commit including dev dependent packages with release type 'none'

## 3.0.1

### Patch Changes

- [`52a88ce`](https://github.com/atlassian/changesets/commit/52a88ce816692f6b18fa8f3f67d707b78b0b8210) [#361](https://github.com/atlassian/changesets/pull/361) Thanks [@Blasz](https://github.com/Blasz)! - Fix dependency release lines being output when they were skipped via the updateInternalDependencies config option

## 3.0.0

### Major Changes

- [`2b49d66`](https://github.com/atlassian/changesets/commit/2b49d668ecaa1333bc5c7c5be4648dda1b11528d) [#358](https://github.com/atlassian/changesets/pull/358) Thanks [@Blasz](https://github.com/Blasz)! - Add new updateInternalDependencies config option to disable auto bumping of internal dependencies in the same release if the dependency was only patch bumped

### Patch Changes

- Updated dependencies [[`89f0c49`](https://github.com/atlassian/changesets/commit/89f0c497ac21b8d008da67caff8032947836c7b1), [`2b49d66`](https://github.com/atlassian/changesets/commit/2b49d668ecaa1333bc5c7c5be4648dda1b11528d), [`09f62f9`](https://github.com/atlassian/changesets/commit/09f62f9c822f31899a48cbd93c7801d72a80b97e)]:
  - @changesets/git@1.0.5
  - @changesets/types@3.0.0
  - @changesets/config@1.1.0

## 2.0.2

### Patch Changes

- [`3dbab2e`](https://github.com/atlassian/changesets/commit/3dbab2e80d9a8a0cccc02d74c6d8150f603219e6) [#343](https://github.com/atlassian/changesets/pull/343) Thanks [@zkochan](https://github.com/zkochan)! - Self-references should be skipped when bumping versions. A self-reference is a dev dep that has the same name as the package. Some projects use self-references as a convinient way to require files using relative paths from the root directory.

## 2.0.1

### Patch Changes

- [`1706fb7`](https://github.com/atlassian/changesets/commit/1706fb751ecc2f5a792c42f467b2063078d58716) [#321](https://github.com/atlassian/changesets/pull/321) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix TypeScript declarations

- Updated dependencies [[`1706fb7`](https://github.com/atlassian/changesets/commit/1706fb751ecc2f5a792c42f467b2063078d58716)]:
  - @changesets/config@1.0.3
  - @changesets/get-version-range-type@0.3.2
  - @changesets/git@1.0.3
  - @changesets/types@2.0.1

## 2.0.0

### Major Changes

- [`011d57f`](https://github.com/atlassian/changesets/commit/011d57f1edf9e37f75a8bef4f918e72166af096e) [#313](https://github.com/atlassian/changesets/pull/313) Thanks [@zkochan](https://github.com/zkochan)! - Bumping `devDependencies` no longer bumps the packages that they depend on.

  This is a pretty big "quality of life" update, which means we will do fewer releases of packages overall, as there is no change of installed packages.

  This has been made a breaking chage as it changes the behaviour of what will be published. It should only be for the better, but we didn't want to surprise you with it.

* [`011d57f`](https://github.com/atlassian/changesets/commit/011d57f1edf9e37f75a8bef4f918e72166af096e) [#313](https://github.com/atlassian/changesets/pull/313) Thanks [@zkochan](https://github.com/zkochan)! - Updates to devDependencies are not affecting the end users of a package. So we are not listing these changes in the changelog file.

### Minor Changes

- [`c3cc232`](https://github.com/atlassian/changesets/commit/c3cc23204c6cb80487aced1b37ebe8ffde0e2111) [#311](https://github.com/atlassian/changesets/pull/311) Thanks [@zkochan](https://github.com/zkochan)! - Added support for workspace ranges. They are now correctly kept and updated when applying a release plan.

### Patch Changes

- [`44555b4`](https://github.com/atlassian/changesets/commit/44555b44cac843d973d31adbfc7703f45117d204) [#315](https://github.com/atlassian/changesets/pull/315) Thanks [@maraisr](https://github.com/maraisr)! - Allows prettier to know about filepaths so it can apply file overrides

- Updated dependencies [[`011d57f`](https://github.com/atlassian/changesets/commit/011d57f1edf9e37f75a8bef4f918e72166af096e)]:
  - @changesets/types@2.0.0
  - @changesets/config@1.0.2
  - @changesets/git@1.0.2

## 1.0.1

### Patch Changes

- [`04ddfd7`](https://github.com/atlassian/changesets/commit/04ddfd7c3acbfb84ef9c92873fe7f9dea1f5145c) [#305](https://github.com/atlassian/changesets/pull/305) Thanks [@Noviny](https://github.com/Noviny)! - Add link to changelog in readme

* [`b49e1cf`](https://github.com/atlassian/changesets/commit/b49e1cff65dca7fe9e341a35aa91704aa0e51cb3) [#306](https://github.com/atlassian/changesets/pull/306) Thanks [@Andarist](https://github.com/Andarist)! - Ignore `node_modules` when glob searching for packages. This fixes an issue with package cycles.

* Updated dependencies [[`04ddfd7`](https://github.com/atlassian/changesets/commit/04ddfd7c3acbfb84ef9c92873fe7f9dea1f5145c), [`e56928b`](https://github.com/atlassian/changesets/commit/e56928bbd6f9096def06ac37487bdbf28efec9d1), [`b49e1cf`](https://github.com/atlassian/changesets/commit/b49e1cff65dca7fe9e341a35aa91704aa0e51cb3)]:
  - @changesets/config@1.0.1
  - @changesets/get-version-range-type@0.3.1
  - @changesets/git@1.0.1
  - @changesets/types@1.0.1

## 1.0.0

### Major Changes

- [`cc8c921`](https://github.com/atlassian/changesets/commit/cc8c92143d4c4b7cca8b9917dfc830a40b5cda20) [#290](https://github.com/atlassian/changesets/pull/290) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Accept `Packages` object from `@manypkg/get-packages` instead of `cwd`

### Patch Changes

- Updated dependencies [[`41e2e3d`](https://github.com/atlassian/changesets/commit/41e2e3dd1053ff2f35a1a07e60793c9099f26997), [`cc8c921`](https://github.com/atlassian/changesets/commit/cc8c92143d4c4b7cca8b9917dfc830a40b5cda20), [`cc8c921`](https://github.com/atlassian/changesets/commit/cc8c92143d4c4b7cca8b9917dfc830a40b5cda20), [`cc8c921`](https://github.com/atlassian/changesets/commit/cc8c92143d4c4b7cca8b9917dfc830a40b5cda20), [`2363366`](https://github.com/atlassian/changesets/commit/2363366756d1b15bddf6d803911baccfca03cbdf), [`cc8c921`](https://github.com/atlassian/changesets/commit/cc8c92143d4c4b7cca8b9917dfc830a40b5cda20)]:
  - @changesets/types@1.0.0
  - @changesets/git@1.0.0
  - @changesets/config@1.0.0

## 0.4.2

### Patch Changes

- Updated dependencies [[`d08c3b3`](https://github.com/atlassian/changesets/commit/d08c3b309d38090ce4f1b8f62cc6b78a5a04efcf)]:
  - @changesets/get-version-range-type@0.3.0

## 0.4.1

### Patch Changes

- Updated dependencies [[`1282ef6`](https://github.com/atlassian/changesets/commit/1282ef698761c1f634fb409842cc7de6b4d03da4)]:
  - @changesets/get-version-range-type@0.2.0

## 0.4.0

### Minor Changes

- [`fe0d9192`](https://github.com/atlassian/changesets/commit/fe0d9192544646e1a755202b87dfe850c1c200a3) [#236](https://github.com/atlassian/changesets/pull/236) Thanks [@Andarist](https://github.com/Andarist)! - Read also pnpm workspace packages when searching for packages.

### Patch Changes

- [`ef6402c9`](https://github.com/atlassian/changesets/commit/ef6402c9d8dc1832126732dbbafb015b71f57f83) [#252](https://github.com/atlassian/changesets/pull/252) Thanks [@Andarist](https://github.com/Andarist)! - Ensure there is a newline between release lines so the final markdown preserves correct formatting.

* [`503154db`](https://github.com/atlassian/changesets/commit/503154db39fe8ab88a1176e4569c48078bcf5569) [#257](https://github.com/atlassian/changesets/pull/257) Thanks [@Noviny](https://github.com/Noviny)! - Move catch statement so errors are less spammy

* Updated dependencies [[`fe0d9192`](https://github.com/atlassian/changesets/commit/fe0d9192544646e1a755202b87dfe850c1c200a3), [`fe0d9192`](https://github.com/atlassian/changesets/commit/fe0d9192544646e1a755202b87dfe850c1c200a3)]:
  - get-workspaces@0.6.0
  - @changesets/git@0.4.0

## 0.3.1

### Patch Changes

- Updated dependencies [[`bca8865`](https://github.com/atlassian/changesets/commit/bca88652d38caa31e789c4564230ba0b49562ad2), [`bca8865`](https://github.com/atlassian/changesets/commit/bca88652d38caa31e789c4564230ba0b49562ad2)]:
  - @changesets/config@0.3.0
  - @changesets/git@0.3.0

## 0.3.0

### Minor Changes

- [`8f0a1ef`](https://github.com/atlassian/changesets/commit/8f0a1ef327563512f471677ef0ca99d30da009c0) [#183](https://github.com/atlassian/changesets/pull/183) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Add support for prereleases. For more information, see [the docs on prereleases](https://github.com/atlassian/changesets/blob/master/docs/prereleases.md).

### Patch Changes

- Updated dependencies [[`8f0a1ef`](https://github.com/atlassian/changesets/commit/8f0a1ef327563512f471677ef0ca99d30da009c0)]:
  - @changesets/types@0.4.0
  - @changesets/config@0.2.3
  - get-workspaces@0.5.2
  - @changesets/git@0.2.4

## 0.2.3

### Patch Changes

- [`a679b1d`](https://github.com/atlassian/changesets/commit/a679b1dcdcb56652d31536e2d6326ba02a9dfe62) [#204](https://github.com/atlassian/changesets/pull/204) Thanks [@Andarist](https://github.com/Andarist)! - Correctly handle the 'access' flag for packages

  Previously, we had access as "public" or "private", access "private" isn't valid. This was a confusing because there are three states for publishing a package:

  - `private: true` - the package will not be published to npm (worked)
  - `access: public` - the package will be publicly published to npm (even if it uses a scope) (worked)
  - `access: restricted` - the package will be published to npm, but only visible/accessible by those who are part of the scope. This technically worked, but we were passing the wrong bit of information in.

  Now, we pass the correct access options `public` or `restricted`.

- [`da11ab8`](https://github.com/atlassian/changesets/commit/da11ab8a4e4324a7023d12f990beec8c3b6ae35f) [#205](https://github.com/atlassian/changesets/pull/205) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Don't update ranges set to \*/x/X when versioning

- Updated dependencies [[`5ababa0`](https://github.com/atlassian/changesets/commit/5ababa08c8ea5ee3b4ff92253e2e752a5976cd27), [`a679b1d`](https://github.com/atlassian/changesets/commit/a679b1dcdcb56652d31536e2d6326ba02a9dfe62)]:
  - @changesets/config@0.2.2
  - get-workspaces@0.5.1
  - @changesets/types@0.3.1

## 0.2.2

### Patch Changes

- [`72babcb`](https://github.com/atlassian/changesets/commit/72babcbccbdd41618d9cb90b2a8871fe63643601) [#178](https://github.com/atlassian/changesets/pull/178) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix changelog generator options not being provided

- Updated dependencies []:
  - @changesets/git@0.2.3

## 0.2.1

### Patch Changes

- [1ff73b7](https://github.com/atlassian/changesets/commit/1ff73b74f414031e49c6fd5a0f68e9974900d381) [#156](https://github.com/atlassian/changesets/pull/156) Thanks [@mitchellhamilton](https://github.com/mitchellhamilton)! - Fix commits not being obtained for old changesets

* [8c43fa0](https://github.com/atlassian/changesets/commit/8c43fa061e2a5a01e4f32504ed351d261761c8dc) [#155](https://github.com/atlassian/changesets/pull/155) Thanks [@Noviny](https://github.com/Noviny)! - Add Readme

- [0320391](https://github.com/atlassian/changesets/commit/0320391699a73621d0e51ce031062a06cbdefadc) [#163](https://github.com/atlassian/changesets/pull/163) Thanks [@Noviny](https://github.com/Noviny)! - Reordered dependencies in the package json (this should have no impact)

- Updated dependencies [8c43fa0, 0320391, 1ff73b7]:
  - @changesets/get-version-range-type@0.1.1
  - @changesets/git@0.2.1
  - @changesets/types@0.3.0
  - @changesets/config@0.2.1

## 0.2.0

### Minor Changes

- [296a6731](https://github.com/atlassian/changesets/commit/296a6731) - Safety bump: Towards the end of preparing changesets v2, there was a lot of chaos - this bump is to ensure every package on npm matches what is found in the repository.

### Patch Changes

- Updated dependencies [296a6731]:
  - @changesets/config@0.2.0
  - @changesets/get-version-range-type@0.1.0
  - get-workspaces@0.5.0
  - @changesets/git@0.2.0
  - @changesets/types@0.2.0

## 0.1.2

### Patch Changes

- [a15abbf9](https://github.com/changesets/changesets/commit/a15abbf9) - Previous release shipped unbuilt code - fixing that

## 0.1.0

### Minor Changes

- [fded7cce](https://github.com/changesets/changesets/commit/fded7cce) - Initial release
