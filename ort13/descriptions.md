### The examples

1. [`Example 1`](./example1.ipynb): describes a basic pytorch model and how to convert that to an ONNX binary.
2. [`Example 2`](./example2.ipynb): `max` -- Here, the pytorch model takes in an array as input, and computes the `max` of the array
   and outputs a linear function of the `max`
3. [`Example 3`](./example3.ipynb): `argmax` -- Here, the pytorch model takes in an array as input, computes the `argmax` of the array
   and outputs a function of this `argmax`. This solution does not work - the ONNX export yields an ONNXRuntimeError
   complaining about not finding an implementation for Argmax.
4. [`Example 4`](./example4.ipynb): `argmax` -- a workaround for `argmax`
5. [`Example 5`](./example5.ipynb): `argmax counts` -- given an array, find the number of times the `max` element appears in the array.
6. [`Example 6`](./example6.ipynb): `conditionals` -- given an array, branch and output based on whether the first element of the array
   is `> 0` or not.
7. [`Example 7`](./example7.ipynb): `conditionals` -- given an array, branch based on whether _all_ the elements of the array are `> 0`
   or not.
8. [`Example 8`](./example8.ipynb): `progressive evaluation`
