![](https://raw.githubusercontent.com/unton3ton/rebootGPUcurrenttemperaturelimit/refs/heads/main/20000_vgg19_60000_at_iteration_60000.png)

## Sources

* [Как добавить скрипт в автозагрузку Ubuntu?](https://losst.pro/kak-dobavit-skript-v-avtozagruzku-ubuntu)
* [Poweroff or Reboot as normal User](https://unix.stackexchange.com/questions/85663/poweroff-or-reboot-as-normal-user)

# Bonus


## OLLama offline  

* [Installing Ollama offline and loading offline models](https://yelog.org/2024/10/10/install-ollama-offline-english/)
* [qwen2.5-3b-gguf](https://huggingface.co/models?search=qwen2.5-3b-gguf)


* [Команда cp в Linux](https://losst.pro/komanda-cp-v-linux)
* [Install an AI LLM on Your Computer: A Step-by-Step Guide](https://www.adventuresincre.com/how-to-install-llm-locally/)
* [Jan is an open source ChatGPT-alternative that runs 100% offline.](https://jan.ai/)
* [qwen2.5-coder](https://ollama.com/library/qwen2.5-coder)


## совместимость с numpy>2.0 и управление загрузкой GPU из tensorflow  

```python
import numpy as np
np.float_ = np.float64
 
 
import tensorflow as tf
gpu_options = tf.compat.v1.GPUOptions(per_process_gpu_memory_fraction=0.86)
sess = tf.compat.v1.Session(config=tf.compat.v1.ConfigProto(gpu_options=gpu_options))
```
