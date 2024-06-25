Qwen 部署方式

1. 在 HuggingFace 上下载 Qwen2-7B-Instruct 和 Qwen2-72B-Instruct-AWQ 这两个版本的模型

https://huggingface.co/Qwen/Qwen2-7B-Instruct

https://huggingface.co/Qwen/Qwen2-72B-Instruct-AWQ

2. 将下载的模型上传到 S3，然后修改 sagemaker_deploy_qwen2.ipynb 文件中的

'serving.properties' 中的 model_id 路径改为第1步上传的模型的路径

```bash
option.model_id=your s3 path to model
```

3. 按照 sagemaker_deploy_qwen2.ipynb 的步骤一步步执行即可
