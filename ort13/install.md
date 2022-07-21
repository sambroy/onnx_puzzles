## Note
These instructions were up-to-date around May 2020. The reader should be able to use the updated onnxruntime and pytorch packages.

### Installation on Linux/Ubuntu
1. Create a conda environment: `conda create -n ort python=3.6`
2. Install `torch` on the conda environment: `conda install pytorch torchvision cudatoolkit=10.2 -c pytorch` -- this installs
`PyTorch 1.5.0` (as in May 2020).
3. Install `onnxruntime`: `pip install onnxruntime` -- installs `onnxruntime 1.3.0` (as in May 2020)
4. (for ease of use, also install) `conda install ipython`, `conda install jupyter`

### End result
```python
import onnxruntime as ort
import onnx
import torch

ort.__version__ == '1.3.0'
onnx.__version__ == '1.7.0'
torch.__version__ == '1.5.0'
```
