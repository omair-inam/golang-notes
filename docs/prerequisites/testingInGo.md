# Testing in Go

## Test functions in Go

A test in Go must satisfy the following requirements

* The containing file must have a name ending in `_test.go`.
* The function name must begin with `Test`.
* The function must have a parameter of type `*testing.T`.
* The function must have *no* return value.


Here's an example of a testing function:

```go title="Sample test function in Go"
func TestAdd(t *testing.T) {
	t.Parallel()
	var expected float64 = 16
	Actual := calculator.Add(7, 9)
	if expected != Actual {
		t.Errorf("Expected %f, Actual %f", want, got)
	}
}
```