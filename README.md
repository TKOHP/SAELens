# 主要类以及其修改部分
## sae_lens/training/activations_store.py
用于激活值采样和存取
### get_data_loader()
注释其中的在线shuffle功能
## sae_lens/cache_activations_runner.py
运行激活值采样的代码
### __init__
添加了多gpu运行大模型
## sae_lens/load_model.py
### load_model()
添加对金融大模型的运行 ,即添加对model_class_name="LlamaForCausalLM"的判断
