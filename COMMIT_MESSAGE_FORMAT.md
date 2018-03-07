# Commit Message Format

**Contents**

* [Commit Message Format](#commit-message-format)
   - [Examples](#examples)
   - [Message Format](#message-format)
   - [Type](#type)
   - [Scope](#scope)
   - [Subject](#subject)
   - [Body](#body)
   - [Footer](#footer)

## Commit Message Format

### Examples

Appears under "Features" header, pencil subheader:

```
feat(pencil): add 'graphiteWidth' option
```

Appears under "Bug Fixes" header, graphite subheader, with a link to issue #28:

```
fix(graphite): stop graphite breaking when width < 0.1 (#28)
```

Appears under "Performance Improvements" header, and under "Breaking Changes" with the breaking change explanation:

```
perf(pencil): remove graphiteWidth option

BREAKING CHANGE: The graphiteWidth option has been removed. The default graphite width of 10mm is always used for performance reason.
```

The following commit and commit `667ecc1` do not appear in the changelog if they are under the same release.
If not, the revert commit appears under the "Reverts" header.

```
revert: feat(pencil): add 'graphiteWidth' option

This reverts commit 667ecc1654a317a13331b17617d973392f415f02.
```

### Message Format

A commit message consists of a **header**, **body** and **footer**.
The header has a **type**, **scope** and **subject**:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and the **scope** of the header is optional.

### Type

Possible values:
* feat - main feature
* fix - bug fixing type
* perf - improving performance
* docs - changing documentation
* chore - updating grunt tasks etc; CI configs, no production code change
* style - CSS changes & others styles
* refactor
* test - for changes of tests
* bump - for assemblies/releases
* revert

If the prefix is `feat`, `fix` or `perf`, it will appear in the changelog.
However if there is any [BREAKING CHANGE](#footer), the commit will always appear in the changelog.

Other prefixes are up to your discretion. Suggested prefixes are `docs`, `chore`, `style`, `refactor`, `test`
and `bump` for non-changelog related tasks.

### Scope

The scope could be anything specifying place of the commit change. Each project has own set of scopes.

### Subject

The subject contains succinct description of the change:

* use the imperative, present tense: "change" not "changed" nor "changes"
* possible to using russian language as history is being viewed not only developers
* no dot (.) at the end

### Body

Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

### Footer

The footer should contain any information about **Breaking Changes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines.
The rest of the commit message is then used for this.
