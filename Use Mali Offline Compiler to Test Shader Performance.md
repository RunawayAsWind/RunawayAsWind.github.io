# Use Mali Offline Compiler to Test Shader Performance

Mali Offline Compiler[^MaliOfflineCompiler] is an official development tool provided by Arm for its Mali series GPUs. Its core function is to pre-compile OpenGL ES or Vulkan shader code into Mali GPU binaries on your computer and generate detailed performance analysis reports.

1. You can use the Mali Offline Compiler or Shader-Playground[^ShaderPlayground]

2. How to obtain the GLSL translated by RenderDoc: On an Android phone, take a screenshot in the app, then click View to obtain the GLSL code.

<img src="./Images/Use Mali Offline Compiler to Test Shader Performance/MaliOfflineCompiler1.png" alt="MaliOfflineCompiler1">

The Edit function also allows for real-time modification of the compiled shader for debugging, such as changing the default precision: 
`precision highp float --> precision mediump int;`

4. If you are using Shader-Playground, just put glsl in it.

5. If using the Mali offline compiler, you can first visit NoteBookCheck[^NoteBookCheck] to learn about Mali chips with performance comparable to the target phone model's chip. This website has test data for different mobile phone chips.

<img src="./Images/Use Mali Offline Compiler to Test Shader Performance/MaliOfflineCompiler2.png" alt="MaliOfflineCompiler2">

6. For example, the OPPO A57 uses the Adreno 505 chip, which, according to the website mentioned above, is comparable to the Mali T860: <https://www.notebookcheck.net/Mali-T860-MP2-vs-Adreno-505_7293_7444.247598.0.html>

<img src="./Images/Use Mali Offline Compiler to Test Shader Performance/MaliOfflineCompiler3.png" alt="MaliOfflineCompiler3">

7. After selecting the Mali chip, go to Mali Offline Compiler official website to install the Mali offline compiler. Enter the command `malioc XXXX.glsl -c Mali-T860` in the console to obtain the performance data of the GLSL code on that chip.

<img src="./Images/Use Mali Offline Compiler to Test Shader Performance/MaliOfflineCompiler4.png" alt="MaliOfflineCompiler4">

[^MaliOfflineCompiler]: Mali Offline Compiler：<https://developer.arm.com/Tools%20and%20Software/Mali%20Offline%20Compiler>

[^ShaderPlayground]: Shader Playground：<https://shader-playground.timjones.io/>

[^NoteBookCheck]: NoteBookCheck：<https://www.notebookcheck.net/ARM-Mali-T860-MP2-Benchmarks-and-Specs.163318.0.html>
