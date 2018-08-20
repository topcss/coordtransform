# 坐标转换模块 coordtransform

此模块用于百度坐标系(bd-09)、火星坐标系(国测局坐标系、gcj02)、WGS84坐标系的相互转换，并提供中文地址到坐标的转换功能，仅使用 C# 标准模块，无其他依赖。

参照 [python的版本](https://github.com/wandergis/coordTransform_py)

## 使用说明

``` CSHARP
var lng = 128.543;
var lat = 37.065;

var result1 = Coordtransform.Gcj02tobd09(lng, lat);// 火星坐标系->百度坐标系
var result2 = Coordtransform.Bd09togcj02(lng, lat);// 百度坐标系->火星坐标系
var result3 = Coordtransform.Wgs84togcj02(lng, lat);// WGS84坐标系->火星坐标系
var result4 = Coordtransform.Gcj02towgs84(lng, lat);// 火星坐标系->WGS84坐标系
var result5 = Coordtransform.Bd09towgs84(lng, lat);// 百度坐标系->WGS84坐标系
var result6 = Coordtransform.Wgs84tobd09(lng, lat);// WGS84坐标系->百度坐标系
```
