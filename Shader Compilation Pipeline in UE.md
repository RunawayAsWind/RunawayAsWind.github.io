# Shader Compilation Pipeline in UE

# How to Debug it?

We can start the first breakpoint from FMaterial::BeginCompileShaderMap. The internal FHLSLMaterialTranslator MaterialTranslator will translate the material graph and fill into MaterialTemplate.

The following diagram illustrates the compilation process of shaders.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile1.png" alt="ShaderCompile1">

The breakpoints below are GetDependentShaderAndVFTypes 

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile8.png" alt="ShaderCompile8">

You can find SortedMeshMaterial below.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile7.png" alt="ShaderCompile7">

The breakpoints below are the starting points of the translation.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile2.png" alt="ShaderCompile2">

The following breakpoints use MaterialTemplate.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile3.png" alt="ShaderCompile3">

After the translation is complete, you can see that the Material Graph has been filled into the MaterialTemplate, forming /Engine/Generated/Material.ush.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile4.png" alt="ShaderCompile4">

/Engine/Generated/UniformBuffers/Material.ush is generated here.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile5.png" alt="ShaderCompile5">

VertexFactory's ModifyCompilationEnvironment is used here.

<img src="./Images/Shader Compilation Pipeline in UE/ShaderCompile6.png" alt="ShaderCompile6">