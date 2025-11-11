# Shader Compilation Pipeline in UE

# How to Debug it?

We can start the first breakpoint from FMaterial::BeginCompileShaderMap. The internal FHLSLMaterialTranslator MaterialTranslator will translate the material map in the UE Editor.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile1.png" alt="ShaderCompile1">

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile2.png" alt="ShaderCompile2">

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile3.png" alt="ShaderCompile3">

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile4.png" alt="ShaderCompile4">

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile5.png" alt="ShaderCompile5">