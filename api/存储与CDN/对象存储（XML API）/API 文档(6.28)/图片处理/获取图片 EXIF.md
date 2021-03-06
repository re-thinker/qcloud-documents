## 功能描述
EXIF（Exchangeable Image File）全称为可交换图像文件，可记录数码照片的拍摄参数、缩略图及其他属性信息。COS 通过数据万象的 **exif** 接口获取 EXIF 信息。目前支持大小在20M以内、长宽小于9999像素的图片处理。


>!如图片无 exif 信息，将返回`{"error" : "no exif data"}`。

## 接口形式

```
download_url?exif
```

## 参数说明

**操作名称**：exif。

| 参数         | 描述                                                         |
| ------------ | ------------------------------------------------------------ |
| download_url | 文件的访问链接，具体构成为`<BucketName-APPID>.cos.<picture region>.<domain>.com/<picture name>`，<br>例如`examplebucket-1250000000.cos.ap-shanghai.myqcloud.com/picture.jpeg`。 |


## 实际案例
```
http://examples-1251000004.cos.ap-shanghai.myqcloud.com/sample.jpeg?exif
```

