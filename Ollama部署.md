Ollama下载：https://ollama.com/download

Ollama模型下载：https://ollama.com/library

Ollama控制台启动命令：`ollama run qwen2`



Anaconda下载：https://www.anaconda.com/download

1.1安装后打开Anaconda Navigator，点击Environment，点击Create

1.2Python版本设置为3.10

1.3设置环境名称为`open-llm-vtuber`

1.4等待导入完成

1.5在Environment中选中`open-llm-vtuber`，在右侧下拉选项选择All，然后搜索websockets，勾选后点击Apply



控制台版：

```
conda create --name open-llm-vtuber python=3.10.13
```

```
conda activate open-llm-vtuber
```



安装依赖：

```
pip install -r requirements.txt
```

```
pip install websockets
```

```
pip install funasr
```

```
pip install torch
```

```
pip install torchaudio
```

```
pip install modelscope
```



安装EdgeTTS：

```
pip install edge-tts
```



重装numpy：

```
pip install --force-reinstall -v "numpy==1.25.2"
```



ffmpeg安装（有则跳过）：

1.1打开Anaconda Navigator

1.2在Environment中选中`open-llm-vtuber`，在右侧下拉选项选择All，然后搜索ffmpeg，勾选后点击Apply



运行服务:

运行Anaconda Prompt

切换环境：

```
conda activate open-llm-vtuber
```

导航到项目目录

运行服务端：

```
python server.py
```

运行主服务：

```
python main.py
```

