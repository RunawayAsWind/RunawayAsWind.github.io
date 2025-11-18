# Get Shader Permutations in your Project

1. Add `r.ShaderPipelineCache.Enabled=True` under `[/Script/Engine.RendererSettings]` in `DefaultEngine.ini`.

2. Add `NeedsShaderStableKeys=True` under `[DevOptions.Shaders]` in `DefaultEngine.ini`.

Then, packaging will generate the following files:

<img src="./Images/Get Shader Permutations in your Project/ShaderStableKeys1.png" alt="ShaderStableKeys1">

The file shows the shader permutations that Cook has incorporated into the package. This CSV file can be processed using Python to obtain relevant information about the shaders.

<img src="./Images/Get Shader Permutations in your Project/ShaderStableKeys2.png" alt="ShaderStableKeys2">