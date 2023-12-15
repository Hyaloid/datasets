## First, download .tar and save them in `$(pwd)/imagenet` folder or else where

```shell
wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_img_train.tar --no-check-certificate

wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_img_val.tar --no-check-certificate

wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_devkit_t12.tar.gz --no-check-certificate
```

## Then, create a virtual env and get all requirements ready

```shell
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113

pip install -r requirements.txt
```

## Finally, use scripts to handle .tar

```python
python download_imagenet.py --data_dir $(pwd)/imagenet
```
