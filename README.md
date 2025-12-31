# Web GPU（Web图形化处理器）
**🏡WebGPU 理论基础：**[https://webgpufundamentals.org](https://webgpufundamentals.org)

**🏡WebGPU 所有核心：**[https://surma.dev/things/webgpu](https://surma.dev/things/webgpu)

**🏡原始WebGPU：**[https://alain.xyz/blog/raw-webgpu](https://alain.xyz/blog/raw-webgpu)



**🏡WebGPU 代码示例：**[https://webgpu.github.io/webgpu-samples](https://webgpu.github.io/webgpu-samples/?sample=helloTriangle)

**🏡WebGPU 最佳做法：**[https://toji.dev/webgpu-best-practices](https://toji.dev/webgpu-best-practices)



**🏡WebGPU 规范：**[https://gpuweb.github.io/gpuweb](https://gpuweb.github.io/gpuweb)

**🏡WGSL 语言规范：**[https://gpuweb.github.io/gpuweb/wgsl](https://gpuweb.github.io/gpuweb/wgsl)



## 什么是Web GPU?

WebGPU是一种新兴的[API](https://baike.baidu.com/item/API/10154?fromModule=lemma_inlink)，它提供对网络上硬件的图形和计算能力的访问。它是在W3C GPU for the Web组内由所有主要浏览器供应商以及英特尔和其他一些公司从头开始设计的，遵循安全，可移植，高性能，可用性。WebGPU旨在在现代图形API（如[Vulkan](https://baike.baidu.com/item/Vulkan/17543632?fromModule=lemma_inlink)、D3D12和[Metal](https://baike.baidu.com/item/Metal/10917053?fromModule=lemma_inlink)）之上工作，其构造反映了这些低级API的基本原语。

WebGPU将物理GPU硬件视为GPUAdapters，通过GPUDevice设备管理资源并执行命令。设备可能拥有自己的内存，能够高速访问处理单元，并包含着色器代码等资源。



WebGPU 是一个应用程序接口，可让您做两件基本的事情。

1. [绘制三角形/点/线到纹理上](https://webgpufundamentals.org/webgpu/lessons/zh_cn/webgpu-fundamentals.html#a-drawing-triangles-to-textures)
2. [在 GPU 上进行计算](https://webgpufundamentals.org/webgpu/lessons/zh_cn/webgpu-fundamentals.html#a-run-computations-on-the-gpu)

就是这样！ 之后有关 WebGPU 的一切都取决于您。这就像学习 JavaScript、Rust 或 C++ 等计算机语言一样。首先要学习基础知识，然后才能创造性地使用这些基础知识来解决问题。

WebGPU 是一个极其低层次的 API. 虽然您可以制作一些小型示例，但对于许多应用程序来说，这可能需要大量代码和大量数据。 举例来说，支持 WebGPU 的 [three.js](https://threejs.org/) 包含约 600k 的 JavaScript，这还只是它的基础库。这还不包括加载器、控件、后处理和许多其他功能。 同样的, [带有 WebGPU 后端的 TensorFlow](https://github.com/tensorflow/tfjs/tree/master/tfjs-backend-webgpu)也需要大约 500K 的 JavaScript 压缩包。

重点是，如果你只想在屏幕上显示一些东西，那么选择一个能提供大量基础代码的库会好得多。



![WebGPU](https://webgpufundamentals.org/webgpu/lessons/resources/webgpu-draw-diagram.svg)
