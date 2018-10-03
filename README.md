# go-performance-tools

This article is about giving a brief overview about the various techniques used to improve the performance of Go program.

After writing your code in Go, before doing anything first thing is to ask question: **does the program build at all**?

This is because there is no point in doing anything further if a binary can’t be built from your Go program.

So we check if it builds by the command:

`go build .`

This should create a binary in go/bin

Once this is checked, next is to check if your Go program gives the correct output. This can be checked by writing tests. Then we execute the test file:

`go test .`

Now that the program successfully builds AND gives the correct expected output, then it makes sense to check its performance. So now we can ask the question: How fast does it run and how much memory does it allocate?

Answer to this lies in benchmark.
