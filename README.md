# conftest-action

This GitHub Action runs [Open Policy Agent](https://github.com/open-policy-agent) [conftest](https://github.com/open-policy-agent/conftest).

## Inputs

## `args`

**Required** Arguments to conftest. e.g. "test -p policy/k8s.rego manifests/*.yaml -o table"

## Outputs

None. Job fails if conftest returns non-zero.

## Example usage

```github
uses: highb/conftest-action@v1.0.0
with:
  args: 'conftest test -p policy/k8s.rego manifests/*.yaml -o table'
```
