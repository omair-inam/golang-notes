---
sidebar_position: 2
---
# First Steps

## Create a new module

```go title="Shell command"
go mod init MODULE_NAME
```

* Go organizes code into *modules*.
* Each module resides in a separate folder.
* Each module must have a `go.mod` file.

## Running tests

```go title="Shell Command"
go test
```

```text title="Shell Output"
PASS
ok      calculator    0.683s
```

## Variable assignment

```go title="Variable assignment syntax"
var VARIABLE_NAME DATA_TYPE = VALUE
```

```go title="Variable assignment sample"
var discount float64 = 4.2
```

## Formatting code

* Use `gofmt`

```text title="gofmt help"
usage: gofmt [flags] [path ...]
  -cpuprofile string
    	write cpu profile to this file
  -d	display diffs instead of rewriting files
  -e	report all errors (not just the first 10 on different lines)
  -l	list files whose formatting differs from gofmt's
  -r string
    	rewrite rule (e.g., 'a[b:len(a)] -> a[b:]')
  -s	simplify code
  -w	write result to (source) file instead of stdout
```

```shell title="List violations (diff)"
gofmt -d FILENAME.go
```

:::tip
VSCode with the Go extension automatically reformats a Go file upon save
:::
