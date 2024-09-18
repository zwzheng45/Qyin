# Qyin

Read this in [<u>EN</u>|[ZH](README_zh.md)]   

<p>
    Try the demo: <a target="_blank" href="https://colab.research.google.com/github/zwzheng45/Qyin/blob/main/%E9%80%9A%E5%BE%8B%E5%8D%83%E9%9F%B3.ipynb">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>
</p>  

Download pre-trained model on [🤗Hugging Face](https://huggingface.co/ZZW45/Qyin)   

## About

Qyin is a model for music score generation and it's based on [Qwen2-7B model](https://github.com/QwenLM/Qwen2).   

It generates the music score in ABC notation and then can be converted into MIDI files by [abcmidi](https://sourceforge.net/projects/abcmidi/), then into any sound format that is available on this planet.   

[MidiCaps](https://huggingface.co/datasets/amaai-lab/MidiCaps) was used for training dataset for this model. Preprocess scripts will be shared later in this repo.   

## Hardware requirements

This model is trained using 3\*A100 80G. 5\*L20 48G also works with a lower batch size and deepspeed enabled.

It's recommonded to have minimum 16GB video memory to run inference using this model.