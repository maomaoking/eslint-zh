---
title: Rule space-return-throw-case
layout: doc
---
<!-- Note: No pull requests accepted for this file. See README.md in the root directory for details. -->

# Require spaces following `return`, `throw`, and `case` (space-return-throw-case)

**Replacement notice**: This rule was removed in ESLint v2.0 and replaced by [keyword-spacing](keyword-spacing) rule.

Require spaces following `return`, `throw`, and `case`.

**Fixable:** This rule is automatically fixable using the `--fix` flag on the command line.

## Rule Details

The following patterns are considered problems:

```js
/*eslint space-return-throw-case: 2*/

throw{a:0}

function f(){ return-a; }

switch(a){ case'a': break; }
```

The following patterns are not considered problems:

```js
/*eslint space-return-throw-case: 2*/

throw {a: 0};

function f(){ return -a; }

switch(a){ case 'a': break; }
```

## Version

This rule was introduced in ESLint 0.1.4 and removed in 2.0.0-beta.3.

## Resources

* [Documentation source](https://github.com/eslint/eslint/tree/master/docs/rules/space-return-throw-case.md)
