# Qyin

Read this in [<u>EN</u>|[ZH](README_zh.md)]   

<p>
    Try the demo: <a target="_blank" href="https://colab.research.google.com/github/zwzheng45/so-vits-svc/blob/32k/%E2%80%9Csovits3_0%E4%B8%80%E9%94%AE%E8%84%9A%E6%9C%AC_ipynb%E2%80%9D%E7%9A%84%E5%89%AF%E6%9C%AC.ipynb">
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