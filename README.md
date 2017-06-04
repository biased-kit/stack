# stack

Package stack implements utilities to capture, manipulate, and format call
stacks. It provides a simpler API than package runtime.

Package stack's types implement fmt.Formatter, which provides a simple and flexible way to declaratively configure formatting when used with logging or error tracking packages.

It was forked from https://github.com/go-stack/stack in order to add an ability to utilize already existed program counters (pc). 
For this goal two functions were added:
 * NewCall(pc int) Call
 * NewCallStack(pcs []int) CallStack

For other details find out original documentation at https://github.com/go-stack/stack