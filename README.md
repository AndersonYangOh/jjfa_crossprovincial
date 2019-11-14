# 基于reactnative跨省流程管理系统
## 一、项目初始化
### 1.创建项目
* react-native init 项目名
### 2.目录结构
* `node_modules/           RN依赖库文件夹`
    `|___package.json            打包脚本，依赖库版本管理文件``
    `|___yarn.lock               依赖库lock文件``
    `|___app.json                app信息文件`
    `|___index.js                RN项目入口文件`
    `|___App.js                  项目文件`
### 3.入口文件
// step 1.引入RN的注册组件API
import { AppRegistry } from 'react-native';
// step 2.引入项目根组件
import App from './App';
// step 3.注册项目根组件
AppRegistry.registerComponent("LearnRN", () => App);
## 二、项目功能说明
### 跨省支撑申请
![image](https://github.com/ChinaUnicomRI/jjfa_crossprovincial/blob/master/b5.jpg)
* 填写商机信息，关联商机号
* 明确客户经理、金额等敏感
* 提交上级审核
* 上级审核后向集团申请
* 集团审核后向其他省分进行分发
* 接收商机的省分进行商机处理
* 商机线下处理，线上上传辅助资料
* 商机完成后，发送商机支撑的用户进行打分
* 系统根据完成状态和流程以及评分，给于一定奖励

