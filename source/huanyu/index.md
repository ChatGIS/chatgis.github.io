---
title: HuanYu
date: 2025-01-01 06:18:10
toc: false
---
该库主要用于提供GIS地图前端开发常用API，包括二维地图、三维地图以及与地图相关的算法API。  
The repository is used to provide common APIs for GIS map front-end development, including 2D map, 3D map, and map-related algorithm APIs.  

**HuanYu**取自《太平寰宇记》中的“寰宇”二字，与天地、乾坤同义，意指整个宇宙、整个空间。
> **《太平寰宇记》** 是古代中国地理志史，记述了宋朝的疆域版图。广泛引用历代史书、地志、文集、碑刻、诗赋以至仙佛杂记等，计约二百种，且多注明出处，保留了大量珍贵的史料。宋太宗赵炅时地理总志；乐史撰，二百卷，是一部现存较早较完整的**地理**总志。  


## 一、开始 Getting Started
Install the [`huanyu` package](https://www.npmjs.com/package/huanyu):

```
npm i huanyu
```

Import huanyu for your application:
```js
import * as huanyu from 'huanyu'

const huanyuFuncTest = () => {
    console.log(huanyu.hello())
}
```

## 二、功能列表 API List
### 1. Hello HuanYu
- hello: 输出Hello HuanYu!
### 2. GIS常用数值
- EarthRadius: 地球平均半径(单位：米)
### 3. 坐标转换
- convertWGS84ToGCJ02: WGS84转GCJ02
- convertGCJ02ToWGS84: GCJ02转WGS84
- convertGCJ02ToBD09: GCJ02转BD09
- convertBD09ToGCJ02: BD09转GCJ02
- convertWGS84ToBD09: WGS84转BD09
- convertBD09ToWGS84: BD09转WGS84
### 4. 计算工具
- getDistance: 计算两点之间大圆距离(Haversine公式)
- getDistancePlus: 计算两点之间大圆距离（Vincenty公式，更精确）
### 5. 数学工具
- toRadians: 角度转弧度
- toDegrees: 弧度转角度
### 6. 颜色工具
- BrandColors: 品牌Logo颜色
- ColorThemes: 颜色主题
- getRandomColorFromTheme: 从主题中获取随机颜色
- getRandomHexColor: 获取随机十六进制颜色
- getRandomRGBColor: 获取随机RGB颜色
- getRandomRGBAColor: 获取随机RGBA颜色
- createColorArray: 创建颜色数组
- isValidColor: 校验颜色是否合法
- convertHexToRGB: 十六进制颜色转RGB
- convertRGBToHex: RGB颜色转十六进制
- convertRGBToRGBA: RGB颜色转RGBA颜色
- convertRGBAToRGB: RGBA颜色转RGB颜色
### 7. 数据类型工具
- wkt2CoorArray: wkt转坐标数组,支持点、线、面(暂不支持多点多线多面)
- wkt2CoorArrayStr: wkt转坐标数组字符串,支持点、线、面(暂不支持多点多线多面)

