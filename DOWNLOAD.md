Dataset **VSAI** can be downloaded in Supervisely format:

 [Download](https://assets.supervisely.com/supervisely-supervisely-assets-public/teams_storage/P/z/EK/UrkLbSTmki4kYQnasRQFgApitPt7KmPnyHyyUMokncJB88y50Xe9UUUWOB19Nb1vn42jlVxJ38P7hzqLVHPkIOBZMwAFyuUJ9KkdbFCaNDhMiuioti9528aIKYvI.tar)

As an alternative, it can be downloaded with *dataset-tools* package:
``` bash
pip install --upgrade dataset-tools
```

... using following python code:
``` python
import dataset_tools as dtools

dtools.download(dataset='VSAI', dst_path='~/dtools/datasets/VSAI.tar')
```
The data in original format can be 🔗[downloaded here](https://www.kaggle.com/datasets/dronevision/vsaiv1/download?datasetVersionNumber=2)