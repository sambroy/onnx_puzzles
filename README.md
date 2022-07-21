# onnxruntime puzzles

Collection of puzzles to implement using onnxruntime.

## Note

These examples were created some time back (Apr-May2020) - I needed to convert my PyTorch models to ONNX, and for that had to use [onnxruntime (shortened as ort)](https://onnxruntime.ai/), also see [github repo](https://github.com/microsoft/onnxruntime).

Around that time, the version available was ORT1.3 and some ops that were in the ONNX spec were not
yet available in the ORT; consequently we had to devise appropriate workarounds. For example, have a
look at the workaround for [argmax](./ort13/example4.ipynb).

The TL;DR of the examples is that many of the ops can be handled via _masking_. Note that some of these workarounds might not be needed any more for the more recent versions of the ORT. I have not looked at the more recent versions of the ORT and the examples here are a guide as to what to do in
case an op implementation is currently missing.

## Background

- What is ONNX? It is a _spec_ -- eg. refer to this [paperspace blog](https://blog.paperspace.com/what-every-ml-ai-developer-should-know-about-onnx/)
- What is onnxruntime? Defined in [onnxruntime.ai](https://onnxruntime.ai/docs/)
