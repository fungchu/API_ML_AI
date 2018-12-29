# API_ML_AI
| Target release  | 2018/11/15  |
| ------------ |------------ |
|  Epic | 刷脸考勤  |
|  Document Status | 已完成   |
|  Document owner |  朱凤 |


文档名称 | 修订日期 |修改内容
 -----| --- | --- 
刷脸考勤1.0 | 2018/11/15| 基本内容框架
轻松考勤2.0 | 2018/11/30|增加用户需求与原型图
轻松考勤3.0 | 2018/12/05|增加精品分析、用户痛点，改变整体论述架构
轻松考勤3.0 | 2018/12/06|增加api输入与输出


## 1.产品分析
### 1.1产品介绍
轻松考勤APP是一款专门为教师设计的，方便教师课堂考勤的人工智能AI应用产品

### 1.2产品目标:
1.轻松考勤，节约时间，减轻老师的负担

2.精准考勤，高效高质，提高管理的质量
### 1.3产品背景：
目前的考勤方式主要是可以分为两种：全点和抽点
前者虽然相对全面，但因为学生基数大，需要花费大量的课堂时间，压缩课堂内容，这显然会影响教学效果。且及时是全点，也同样可能会遭遇代课代达到的情况。

抽点虽然减少了点名的时间，但同样会出现也同样可能会遭遇代课代达到的情况，以及有所谓的幸运儿没到课但也没被发现的情况。针对这两困境，我们提出刷脸考勤，每个人的脸即便是双胞胎也不可能完全一样，这样可以有效的防止代课。其次自动识别自动考勤，减少考勤在课堂上时间的比重，有足够多时间完成教学任务。
### 1.4用户痛点
目前一般的大学课堂都是强制要求老师点必须对学生进行考勤的，并且将学生的考勤情况++与老师的评优相联系起来++，换言之虽然老师可以不用每节课都点名，但无法避免的是++必须对学生进行一定次数的考勤++。

另一方面，学生的到勤情况很大程度上会影响教学质量，无论是从学风建设上来说，还是从学习吸收知识上来讲都是如此。而教学质量低下则会被认定为教学事故，这会影响到老师的工资收入、评优评先，甚至是晋升机会。

教师的的工资收入、评优评先、晋升机会与学生考勤相联系，然而传统的考勤难以做到便捷快速精准的考勤，这就是用户的痛点。
### 1.5应用场景:
场景一：今天要上课的内容很多，这是一个很大的班，教秘那边又要求老师要给学生考勤，但无疑这会花去大量的时间。这时候通过人脸识别，轻松考勤，节约时间。

场景二：代课现象层出不穷，学校要求上课老师严打代课，可老师也不能保证能够精准的认出每个学生。这时候通过人脸识别，精准考勤，高效高质。
### 1.6同类产品分析
产品名：上朝啦app
![image](https://raw.githubusercontent.com/fungchu/API_ML_AI/gh-pages/image/%E4%B8%8A%E6%9C%9D.png)
特色：首款采用人脸识别的智能考勤app

使用方法：手机定位+人脸识别
员工到达公司后，打开手机的定位系统定在公司，然后自拍上传到系统进行打卡。

不足：目前手机的定位没有办法定位到具体的课室








## 2.使用者交互设计
[产品功能结构图](https://github.com/fungchu/API_ML_AI/blob/master/image/%E5%8A%9F%E8%83%BD%E7%BB%93%E6%9E%84.png?raw=true)
![image](https://raw.githubusercontent.com/fungchu/API_ML_AI/gh-pages/image/%E5%8A%9F%E8%83%BD%E7%BB%93%E6%9E%84.png)
**页面信息流程图**
![image](https://github.com/fungchu/API_ML_AI/blob/master/image/%E9%A1%B5%E9%9D%A2.png?raw=true)





#### 总体逻辑说明
[原型链接](https://fungchu.github.io/qingsongkaqoqin_app)
![引导页](https://github.com/fungchu/API_ML_AI/blob/master/image/%E5%BC%95%E5%AF%BC%E9%A1%B5.png?raw=true)

- 主要有三个功能，从左到右分别是：考勤库、照相、用户；通过底部tab键的点击分别进行主要功能页面的跳转
- 默认进入页面是考勤库

---

#### 登录页面逻辑说明
![image](https://github.com/fungchu/API_ML_AI/blob/master/image/%E7%99%BB%E5%BD%95.png?raw=true)
- 功能权限分为登录/非登陆两个状态

> 登录 -->进入页面可使用APP功能
非登录-->无法使用APP功能   

- 用户通过输入【账号】和【密码】登录，点击【登录】键页面跳转到【考勤库】
- 点击【还没注册】页面跳转到【注册】页面，填入相关信息后，点击【注册】页面跳转回【登录】页面
- 当用户忘记了自己的密码，可以通过点击【找回密码】重新设置密码
#### 登录页面交互说明
- 点击【登录】，按键从蓝色#3c78d8变成红色，#FF4040
- 点击【注册】，按键从蓝色#3c78d8变成红色，#FF4040
- 点击【确认】，按键从蓝色#3c78d8变成红色，#FF4040
- 点击【发送】，按键从白色#ffffff变成灰色，#bbb9b9
---

#### 考勤库逻辑说明
![image](http://m.qpic.cn/psb?/V1416Q0X4NuFBN/vyCdmyHkjpQ6zSbIhpw3gboQI15vWNpwRStwb4UToSw!/b/dEkBAAAAAAAA&bo=UARYAgAAAAADByw!&rf=viewer_4)
- 点击【考勤库】，出现的是以列表形式出现的课程名，这是在用户id与教务系统绑定之后，根据课程安排自动生成的。
- 用户点击【课程名】进入该课程以日期为单位的考勤列表，日期按照上课时间作为排序记录。底部有个【合成】键，点击合成键可自行决定将某几个日期的课程合成到同一个文件中方便查阅。
- 点击【具体日期】出现的是该日期具体每个学生的考勤情况，“打勾”代表到课，“圈圈”代表缺勤。右下角有【分享】键可对考勤情况进行分享。
- 点击【分享】可选择分享的方式：微信、QQ、其他方式；其他方式有以图片/pdf/excel

#### 考勤库交互说明
- 选中【考勤库】，底下图标变成红色，#FF4040
- 点击【课程名】列表颜色降低灰度
- 点击【具体日期】列表钮颜色降低灰度
- 点击【合成】键，按键颜色变成红色#FF4040，跳转页面到合成页面，通过勾选决定具体合成哪几个页面
- 点击【分享】底部弹出抽屉栏框架，依次排列微信、QQ、邮件、其他方式的图标。图标被点击成红色#FF4040


---

#### 照相机逻辑说明
![image](https://github.com/fungchu/API_ML_AI/blob/master/image/%E7%85%A7%E7%9B%B8%E6%9C%BA.png?raw=true)
- 点击【照相机】进入拍摄页面
- 拍照之后可选择“√”和“×”分别对应确定照片和删除照片。选择“×”之后重新进入拍摄页面，进行拍摄。确定照片之后可以进入选择班级的页面，确定要进行照片对比的班级。
#### 照相机交互说明
- 拍照之后确定完照片，跳转到班级选择页面
- 点击【课程名（班级）】列表颜色降低灰度

---
#### 用户页逻辑说明
![image](https://github.com/fungchu/API_ML_AI/blob/master/image/%E7%94%A8%E6%88%B7.png?raw=true)
- 点击【退出登录】会跳转回【登录页面】
- 点击【我的学生】进入【我的学生页面】里面是这个学期该被该老师任教的学生的名单，以列表形式陈列，可通过字母排序进行查找，也可以在搜索框中直接搜索学生。
- 选中所要查询学生的名字，跳转到【选择班级页面】，这个页面会出现该学生这学期被这个老师教的课程名。
> - 例如，老师A和学生B，学生B这学期选了老师A的API课和文献综述课。老师A在【我的学生页面】选中学生B后，【选择班级页面】就会出现老师A的API课和文献综述课。
- 点击你想要查看的课程就会转入【学生名-课程名】页面，这里显示的是这学期该名学生的这门课的考勤情况
#### 用户页交互说明
- 点击【退出登录】键，按键颜色变成红色#FF4040，跳转页面到【登录】页面
- 点击【我的学生】和【关于我们】列表颜色降低灰度
- 选中【我的学生页面】和【选择班级页面】列表颜色降低灰度

## 3.API&AI
### 3.API使用水平
[API技术框架](http://naotu.baidu.com/file/f5b34bbfcc9cc3be99b14cc9b6f3b598?token=3a597425f1ffbf95)

![image](https://raw.githubusercontent.com/fungchu/API_ML_AI/master/image/%E4%BA%BA%E8%84%B8%E6%9F%A5%E6%89%BE%EF%BC%88%E5%AF%B9%E6%AF%94%E7%AD%9B%E9%80%89%EF%BC%89.png)

---


**所需的API：百度AI**
[人脸库](http://ai.baidu.com/docs#/Face-Set/top)
[人脸查找](http://ai.baidu.com/docs#/Face-Search/top)


1. **人脸库-人脸注册**    [技术文档](https://ai.baidu.com/docs#/Face-Set-V3/top)

- 作用：要完成1：N或者M：N识别，首先需要构建一个人脸库，用于存放所有人脸特征。
- 接口描述：用于向人脸库中新增用户，及组内用户的人脸图片
- 请求方法：POST
- 接口地址：https://aip.baidubce.com/rest/2.0/face/v3/faceset

**AipFace**
```
from aip import AipFace

""" 你的 APPID AK SK """
APP_ID = '*****58'
API_KEY = 'a3Z3PWaqe******ene57L'
SECRET_KEY = 'Zd******suLrDdb6iIAyQmNUaAH07a'

client = AipFace(APP_ID, API_KEY, SECRET_KEY)  

#获取百度token（可以理解为密钥）
def get_token(API_KEY, SECRET_KEY):
    import requests
    import json

    payload = {
        'grant_type': 'client_credentials', 
        'client_id': '{}'.format(API_KEY),
        'client_secret': '{}'.format(SECRET_KEY)
    }

    r = requests.post("https://aip.baidubce.com/oauth/2.0/token", data=payload)
    
    return (r.json()['access_token'])
```
**人脸注册**
```
#上传图片到人脸库
image = "https://raw.githubusercontent.com/Tumaorou/face_search/master/yao_ming.jpg"

imageType = "URL"

groupId = "test_group"#用户组

userId = "yao_ming"#用户名，一个用户可注册多张图片

""" 如果有可选参数 """
options = {}
options["user_info"] = "user's info"
options["quality_control"] = "NONE"
options["liveness_control"] = "LOW"

""" 带参数调用人脸注册 """
client.addUser(image, imageType, groupId, userId, options)

```
> {'cached': 0,
 'error_code': 223105,
 'error_msg': 'face is already exist',
 'log_id': 744193254732205361,
 'result': None,
 'timestamp': 1545473220}
 
2.人脸搜索
[技术文档](https://ai.baidu.com/docs#/Face-Search-V3/4804d33e)

- 作用：待识别的图片中，存在多张人脸的情况下，支持在一个人脸库中，一次请求，同时返回图片中所有人脸的识别结果。
- 接口描述：待识别图片中含有多个人脸时，在指定人脸集合中，找到这多个人脸分别最相似的人脸
- 请求方法：POST
- 接口地址：https://aip.baidubce.com/rest/2.0/face/v3/multi-search

```
#获取用户列表
client.getGroupUsers(groupId)
```
> {'cached': 0,
 'error_code': 0,
 'error_msg': 'SUCCESS',
 'log_id': 747956954732228941,
 'result': {'user_id_list': ['zhu_feng', 'yao_ming']},
 'timestamp': 1545473222}
 
```
#获取用户人脸列表
client.faceGetlist('zhu_feng', groupId)
```
> {'cached': 0,
 'error_code': 0,
 'error_msg': 'SUCCESS',
 'log_id': 747956954732232601,
 'result': {'face_list': [{'ctime': '2018-12-16 13:53:02',
    'face_token': 'a0995896f6773b08a3620ddd229d8344'}]},
 'timestamp': 1545473223}
 
```
#人脸搜索
def search_face(API_KEY, SECRET_KEY, img_url):
    import requests
    import json
    
    access_token = str(get_token(API_KEY, SECRET_KEY))
    
    payload = {
        'image': '{}'.format(img_url),
        'image_type' : 'URL',
        'group_id_list': 'test_group',#从指定的group中进行查找 用逗号分隔，上限10个
        "max_face_num" : 5,#最多处理人脸的数目，默认值为1(仅检测图片中面积最大的那个人脸) 最大值10
    }

    r = requests.post('https://aip.baidubce.com/rest/2.0/face/v3/search?access_token='+ access_token, params=payload)

    return (r.json())
```

```
#填写需要查找的图片地址
img_url = 'https://raw.githubusercontent.com/Tumaorou/face_search/master/group.jpg'
 
search_face(API_KEY,SECRET_KEY,img_url)
```
> {'cached': 0,
 'error_code': 0,
 'error_msg': 'SUCCESS',
 'log_id': 747956954732241961,
 'result': {'face_token': '2ee12854f31f8c0700ea9aae8fbc940d',
  'user_list': [{'group_id': 'test_group',
    'score': 16.384712219238,
    'user_id': 'yao_ming',
    'user_info': "user's info"}]},
 'timestamp': 1545473224}

### 3.2 API使用比较分析
#### 3.2.1 价格
Face++
![face++价格图](https://raw.githubusercontent.com/fungchu/API_ML_AI/master/image/face%2B%2B%E4%BB%B7%E6%A0%BC%E5%9B%BE.png)
百度AI
![百度ai价格图](https://raw.githubusercontent.com/fungchu/API_ML_AI/master/image/%E7%99%BE%E5%BA%A6%E4%BB%B7%E6%A0%BC%E5%9B%BE.png)
对比分析

平台 | 技术| 按量计费| 包时计费| 调用失败
---|---|---|---|---
 Face++|人脸识别| 调用+储存+调用失败|1000元/月/QPS   100元/月/QPS|计费
百度AI |人脸识别| 免费|300元/月/QPS   30元/天/QPS|不计费
在双方提供的服务数量相同的情况下，按照包月计费来看，face++在价格上远超百度AI；且按量计费和调用失败的收费上，百度AI的价格更加实惠。

### 3.2 人工智能概率性
![人工智能概率性](https://github.com/fungchu/API_ML_AI/blob/master/image/%E7%99%BE%E5%BA%A6AI%E9%94%99%E8%AF%AF%E8%AF%86%E5%88%AB%E7%8E%87.png?raw=true)


---
## Manlifest
1. [产品功能结构图](https://github.com/fungchu/API_ML_AI/blob/master/image/%E5%8A%9F%E8%83%BD%E7%BB%93%E6%9E%84.png?raw=true)
2. [原型链接](https://fungchu.github.io/qingsongkaqoqin_app)
3. [API技术框架](http://naotu.baidu.com/file/f5b34bbfcc9cc3be99b14cc9b6f3b598?token=3a597425f1ffbf95)
4. [人脸库](http://ai.baidu.com/docs#/Face-Set/top)
5. [人脸查找](http://ai.baidu.com/docs#/Face-Search/top)
