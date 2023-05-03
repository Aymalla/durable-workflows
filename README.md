# Durable-workflows

This repository will demonstrate different alternatives to deliver durable execution for your services and applications and eliminate complex error or retry logic, avoid callbacks, and ensure that every workflow you start, completes.

## Problem statement

For example, we might have three functions that are called in sequence or chained together. Function One gets called first, and when it's finished, it triggers Function Two, and then when that's finished, it triggers Function Three. And, of course, it's possible to implement this with regular Azure Functions. We could use queue messages. So, Function One puts a message on a queue, and that message triggers Function Two, and so on. But what if we wanted to implement a fan-out, and fan-in pattern?

So, Function One might trigger multiple instances of Function Two, and then we want to wait until all of those instances of Function Two have finished, before triggering Function Three. But that's actually quite a lot harder to do, just with regular Azure Functions. Or, going back to the chaining example, what if we wanted to write an error handler, that could handle an error, wherever in the chain it occurred, whether it was in Function One, Two, or Three?
