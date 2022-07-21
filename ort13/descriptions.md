### The examples

1. `Example 1`: describes a basic pytorch model and how to convert that to an ONNX binary.
2. `Example 2`: `max` -- Here, the pytorch model takes in an array as input, and computes the `max` of the array
   and outputs a linear function of the `max`
3. `Example 3`: `argmax` -- Here, the pytorch model takes in an array as input, computes the `argmax` of the array
   and outputs a function of this `argmax`. This solution does not work - the ONNX export yields an ONNXRuntimeError
   complaining about not finding an implementation for Argmax.
4. `Example 4`: `argmax` -- a workaround for `argmax`
5. `Example 5`: `argmax counts` -- given an array, find the number of times the `max` element appears in the array.
6. `Example 6`: `conditionals` -- given an array, branch and output based on whether the first element of the array
   is `> 0` or not.
7. `Example 7`: `conditionals` -- given an array, branch based on whether _all_ the elements of the array are `> 0`
   or not.
8. `Example 8`: `progressive evaluation`
