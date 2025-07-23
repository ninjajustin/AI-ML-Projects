# Unification Algorithm Implementation
This assignment involved implementing the Unification algorithm, a fundamental operation in logic programming and automated reasoning. The goal is to find a substitution that makes two expressions syntactically identical.

Key points:

Expressions are based on S-expressions (LISP-like lists), consisting of:

Constants: starting with uppercase letters or lowercase predicates

Variables: start with a question mark (e.g., ?x, ?yum)

Lists: nested expressions such as (loves Fred Wilma) or (loves ?x ?y)

The unification function recursively attempts to match two expressions by:

Returning empty substitution {} if they are identical constants or empty lists

Binding variables to expressions if no circular references occur (occurs check)

Recursing on sub-expressions when both expressions are lists

Returning failure (None or FAIL) when no unification is possible

The output is either:

None if unification fails,

An empty substitution {} if the expressions are identical without variables,

Or a substitution dictionary mapping variables to values, e.g. {"?x": "Fred"}

This implementation supports unifying expressions with variables in any position, including relation names, and avoids variable capture or infinite loops by using the occurs check.