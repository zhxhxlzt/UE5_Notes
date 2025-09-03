# ShadingModel是如何从材质里设置到最终在Shader中使用的？
![alt text](images/UE5/image-1.png)
ShadingModel 通过在材质中设置后通过Compiler->ShadingModel 写入CodeTrunk
![alt text](images/UE5/image-2.png)
没有使用MSM_FromExpression时，会走else分支
![alt text](images/UE5/image-3.png)
![alt text](images/UE5/image-4.png)
BasePass Shader中获取ShadingModel的地方
![alt text](images/UE5/image-5.png)
ShadingModel的写入是在材质编译生成的代码中的
![alt text](images/UE5/image-6.png)
![alt text](images/UE5/image-7.png)
![alt text](images/UE5/image-8.png)
![alt text](images/UE5/image-9.png)
![alt text](images/UE5/image-10.png)