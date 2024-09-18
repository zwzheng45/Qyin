# 通律千音

Read this in [[EN](README.md)|<u>ZH</u>]   

<p>
    试试demo：<a target="_blank" href="https://colab.research.google.com/github/zwzheng45/Qyin/blob/main/%E9%80%9A%E5%BE%8B%E5%8D%83%E9%9F%B3.ipynb">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>
</p>  
从 [🤗Hugging Face](https://huggingface.co/ZZW45/Qyin) 下载预训练模型

## 关于

通律千音是基于[通义千问Qwen2-7B](https://github.com/QwenLM/Qwen2)的乐谱生成大模型。

本模型生成ABC记谱法表示的音乐，并能被[abcmidi](https://sourceforge.net/projects/abcmidi/)这类工具转换成通用MIDI文件，然后可以再转换成这个地球上存在的任何一种音频格式。

通律千音使用了[MidiCaps](https://huggingface.co/datasets/amaai-lab/MidiCaps)数据集用于训练。预处理脚本将会在晚些时候上传到这个仓库。

## 硬件需求

本模型使用了3\*A100 80G进行训练。经测试，调低批大小并使用deepspeed后也能在5\*L20 48G上训练。

推荐使用至少16GB显存的GPU对本模型进行推理。