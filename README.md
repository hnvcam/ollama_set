Fix issue of Docker image: open-webui:cuda: Fails to transcribe audio to text.
- Open shell access to the open-webui container in Docker Desktop by accessing Exec tab.
```
cd /usr/local/lib/python3.11/site-packages/nvidia/cudnn/lib
ln -s libcudnn_ops.so.9 libcudnn_ops_infer.so.8
ln -s libcudnn_cnn.so.9 libcudnn_cnn_infer.so.8
```
