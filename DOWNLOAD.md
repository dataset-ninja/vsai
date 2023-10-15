Dataset **VSAI** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/supervisely-supervisely-assets-public/teams_storage/M/b/AB/tlX3SiVFDQr2KyTvIm17M4Qw9lzGpzQNDZ9376lzUAudzl29H9e0u1jyFAU51DzwzWCp9UoTSBMmvaBYtzJceb5iGLBVjRmdBaVtA416ojyH8s2V0VLgSz0LQ1Jn.tar)

As an alternative, it can be downloaded with *dataset-tools* package:
``` bash
pip install --upgrade dataset-tools
```

... using following python code:
``` python
import dataset_tools as dtools

dtools.download(dataset='VSAI', dst_dir='~/dataset-ninja/')
```
Make sure not to overlook the [python code example](https://developer.supervisely.com/getting-started/python-sdk-tutorials/iterate-over-a-local-project) available on the Supervisely Developer Portal. It will give you a clear idea of how to effortlessly work with the downloaded dataset.

The data in original format can be [downloaded here](https://www.kaggle.com/datasets/dronevision/vsaiv1/download?datasetVersionNumber=2).