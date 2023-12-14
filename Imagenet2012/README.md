# Download datasets

## First, download .tar and save them in `$(pwd)/imagenet` folder

```shell
wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_img_train.tar --no-check-certificate

wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_img_val.tar --no-check-certificate

wget https://image-net.org/data/ILSVRC/2012/ILSVRC2012_devkit_t12.tar.gz --no-check-certificate
```

## Then, use scripts to handle .tar

```python
python download_imagenet.py --data_dir $(pwd)/imagenet
```
