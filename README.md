
# 驾驶护航
| 发布日期 | 2019-12-10 |
| -------- | --------- |
| 项目名称 | 驾驶护航 |
| 项目状态 | 进行中 |
| 项目设计 | 周沛文 |
| 项目负责人 | 周沛文 |
## 价值主张
### 背景
2018年8月24日，一名女子乘坐滴滴遭遇奸杀，期间其好友发现不妥在滴滴软件对滴滴客服进行线上询问时，客服一直答复“请您耐心等待”“我们尽快处理”，没有得到有效的正面回答。一夜过去，25号女子尸体在悬崖被发现。此事引起全网轰动和谴责。滴滴自此关闭滴滴顺风车服务。
### 加值宣言 
驾驶护航是一个结合了驾驶行为分析API和危险行为识别API的产品，稳定、低成本、高效率、地为不同群体的司机及乘客提供安全保障。产品测试稳定后可以推广到旅汽及运营车辆公司大范围使用。

### 核心价值（最小可行性产品）
* 导航路线
* 识别出司机不规范驾驶时发出警报
* 出现斗殴、推打的时候，给乘客提供快捷有效报警的方式。


### 用户痛点 
1.用户想要尽可能降低自己交通事故的可能性，保障自己行车安全<br>
2.滴滴、嘀嗒等约车用户担心自己乘车安全以及报警不及时有效<br>
3.市面现有的软件（如滴滴）的报警功能十分不主动、延迟、大众对其抱有怀疑、不信任的情绪

### 人工智能概率性与用户痛点
* 视频清晰时辨别准确
* 视频不清晰，肢体模糊或重叠时辨别模糊

  
### 需求列表与人工智能API加值 
| 需求 | 所用API |
| -------- | --------- |
| 规范驾驶行为 | 行为驾驾驶分析 |
| 保障乘客安全 | 危险行为识别 |
| 报警系统 | 语音合成 |
| 路线导航记录路程 | GPS地图 |

### 应用场景
* 司机驾驶时出现抱怨、躁动、砸东西等负面情绪时，发出语音提示“保持心情稳定安全驾驶”
* 司机上车后双手离开方向盘，驾驶护航监控识别到此行为后发出警报语音提示“请注意行车安全”
* 当乘客之间和与司机之间出现危险行为时（殴打、拉扯）发出警报语音询问是否报警，得到“联系人”“报警”回应后直接扬声播打电话（且一旦开始拨打，手机无法关机）

## 原型 

### 产品框架图
![产品框架图](https://github.com/pumennn/qimo/blob/master/pdf/%E9%A9%BE%E9%A9%B6%E6%B5%81%E7%A8%8B%E5%9B%BE.png)
### 交互及页面设计
![原型](https://github.com/pumennn/qimo/blob/master/pdf/%E5%8E%9F%E5%9E%8B1.png?raw=true)

原型2.信息设计 5%
信息设计：在PRD文件中是否有说明且原型是否有做到：信息设计的某个核心信息或设计使用了人工智能的加值

原型3.原型文档 5%
原型文档：多少程度上有提供MVP可交互的原型文档，供它人在Github上下载使用

### 口头操作说明 
口头操作说明：大家好！经过我们的反复调试及测试，我们的驾驶护航APP现已投入使用。我们团队基于想要减少交通事故、提高司机驾驶安全的想法，设计此款APP，我们结合百度的驾驶行为分析API以外，还结合了危险行为识别的API，危险行为识别API可以识别车内人员出现推打拉扯的行为，也可以识别司机单人时出现抱怨、砸东西等行为，提出警报，并且安排语音合成的报警系统，只需语音回答即刻自动接通报警电话。
## API 产品使用关键AI或机器学习之API的输出入展示 15%
### API1.使用水平

#### 使用比较分析 
* 语音合成：
[阿里云语音合成介绍](https://ai.aliyun.com/nls/tts?spm=a2c4g.750001.h2v3icoap.188.47ca7b13RyG9D7)![阿里云价格](https://github.com/pumennn/qimo/blob/master/pdf/%E9%98%BF%E9%87%8C%E4%BA%91%E8%AF%AD%E9%9F%B3%E5%90%88%E6%88%90%E4%BB%8B%E4%B8%AA.png)<br>
[百度语音合成](https://ai.baidu.com/ai-doc/SPEECH/yk38y8h3j)![百度价格](https://github.com/pumennn/qimo/blob/master/pdf/%E7%99%BE%E5%BA%A6%E8%AF%AD%E9%9F%B3%E5%90%88%E6%88%90%E4%BB%B7%E6%A0%BC.png)<br>
价格上：百度语音单次价格高于阿里云单次价格<br>
功能上：百度语音合成有离线的合成，使用性更高，不受限制<br>

* 地图api:
[高德](https://lbs.amap.com/)<br>
[百度](http://lbsyun.baidu.com/)<br>
[腾讯](https://lbs.qq.com/)<br>
[阿里云](https://yq.aliyun.com/zt/9275)<br>

API3.使用后风险报告 5%
使用后风险报告：在PRD文件中是否有说明且提供连结证据，所使用的API类别的现在及未来发展性，如API市场竞争程度丶输入输出限制丶定价丶及可替代的程序库（改用自己开发的代码及数据库而不用API）等等

API4.加分项 3%
使用复杂度：用了2个以上机器学习与人工智能的API之输入及输出<br>
输入：<br>
```python
""" 读取图片 """
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

image = get_file_content('example.jpg')

""" 调用驾驶行为分析 """
client.driverBehavior(image);

""" 如果有可选参数 """
options = {}
options["type"] = "smoke"

""" 带参数调用驾驶行为分析 """
client.driverBehavior(image, options)
```

输出：<br>
```python
{
  "person_num": 1,
  "person_info": [{
    "attributes": {
      "cellphone": {
        "threshold": 0.9,
        "score": 0.500098466873169
      },
      "both_hands_leaving_wheel": {
        "threshold": 0.9,
        "score": 0.468360424041748
      },
      "not_facing_front": {
        "threshold": 0.9,
        "score": 0.08260071277618408
      },
      "not_buckling_up": {
        "threshold": 0.9,
        "score": 0.998087465763092
      },
      "smoke": {
        "threshold": 0.9,
        "score": 6.29425048828125e-05
      }
    },
    "location": {
      "width": 483,
      "top": 5,
      "height": 238,
      "left": 8
    }
  }],
  "log_id": 2320165720061799596
}
```
