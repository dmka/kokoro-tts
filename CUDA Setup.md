# CUDA Setup

## Install ONNX GPU runtime
```
pip uninstall onnxruntime
pip install "onnxruntime_gpu[cuda,cudnn]"
```

## Set environment variable
`ONNX_PROVIDER=CUDAExecutionProvider`

## Preload CUDA DLLs
```
import onnxruntime as rt
rt.preload_dlls()
```