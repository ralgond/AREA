# LineaRE

## 软硬件环境

PyTorch  2.0.0

Python  3.8(ubuntu20.04)

Cuda  11.8

RTX A5000(24GB) * 1

## 安装与运行
```bash
pip install -r requirements.txt

mkdir -p ./raw_data/ecom-social/

mkdir -p ./data/ecom-social/

mkdir -p ./save/ecom-social/
```

Put raw data into ./raw_data/ecom-social/

```
python process_data2.py

bash run.sh

# wait about 9 hours...
```

The result file is located in ./save/ecom-social/, it's name is submit.json

## 关于结果的随机性
结果会在一定范围里波动，所以请多试几次（多执行几次run.sh，每次大概花费9小时），然后取最大的那个结果即可。
