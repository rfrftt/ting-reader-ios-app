# Ting Reader iOS App

![Logo](./logo.png)

一个基于 [ting-reader](https://github.com/dqsq2e2/ting-reader.git) 后端数据服务的 iOS 听书应用，面向中文有声书场景，提供更轻量、更专注的移动端收听体验。

**需要自行搭建后端服务，需要自行对ipa包签名安装**

可参考 [SideStore 自签名安装说明](https://github.com/SideStore/SideStore) 完成 `ipa` 自签名与安装；免费 Apple ID 签名通常需要定期续签，请参考说明搭配快捷指令自动刷新。

**app提供听书的最小化功能实现,其他管理和扩展功能需要使用web端进行管理。**

[去下载TingReader.ipa](https://github.com/rfrftt/ting-reader-ios-app/releases/tag/alpha) 


## 项目简介

本工程是 `ting-reader` 的 iOS 客户端极简实现，围绕“打开即听”的使用方式，提供书库管理、章节浏览、播放控制、进度续听与个性化设置等核心能力。应用界面以简洁、清爽、易读为主，适合作为个人有声书库的移动端入口。

依托 `ting-reader` 后端的数据管理能力，应用可以更好地组织书籍、章节、作者、演播者等内容信息，并在移动端提供更稳定、更连贯的收听体验。



## 功能特性

- 书库浏览与书籍详情查看
- 章节列表快速切换，支持正文与番外分类查看
- 沉浸式播放界面，支持进度拖动、上一集/下一集、快进快退
- 最近播放与继续播放，方便断点续听
- 收藏管理与搜索入口，提升内容查找效率
- 睡眠定时、倍速播放、片头片尾跳过等常用听书功能
- 自动预加载、自动缓存、主题切换等个性化设置
- 基于后端服务的数据组织与状态管理能力

## 后端数据来源

本项目以前端 iOS App 的形式接入以下后端项目作为数据来源：

- 后端仓库: [dqsq2e2/ting-reader](https://github.com/dqsq2e2/ting-reader.git)

## 界面预览

<table>
  <tr>
    <td align="center" width="50%">
      <strong>首页</strong><br />
      <sub>展示书库统计、最近播放与快速续听入口</sub><br /><br />
      <img src="./snap/IMG_5108.PNG" alt="首页" width="78%" />
    </td>
    <td align="center" width="50%">
      <strong>书籍详情</strong><br />
      <sub>查看作品信息、章节内容与播放进度</sub><br /><br />
      <img src="./snap/IMG_5106.PNG" alt="书籍详情" width="78%" />
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <strong>章节列表</strong><br />
      <sub>支持正文与番外切换，快速定位章节</sub><br /><br />
      <img src="./snap/IMG_5104.PNG" alt="章节列表" width="78%" />
    </td>
    <td align="center" width="50%">
      <strong>播放页(主题光晕)</strong><br />
      <sub>支持倍速、跳转、定时与片头片尾控制</sub><br /><br />
      <img src="./snap/IMG_5103.PNG" alt="播放页" width="78%" />
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <strong>睡眠定时(主题光晕)</strong><br />
      <sub>内置常用定时选项，适合夜间收听场景</sub><br /><br />
      <img src="./snap/IMG_5105.PNG" alt="睡眠定时" width="78%" />
    </td>
    <td align="center" width="50%">
      <strong>设置页</strong><br />
      <sub>提供主题、播放偏好与服务状态配置</sub><br /><br />
      <img src="./snap/IMG_5107.PNG" alt="设置页" width="78%" />
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center" width="33.33%">
      <strong>缓存日志</strong><br />
      <sub>播放页面的缓存日志查看</sub><br /><br />
      <img src="./snap/1.PNG" alt=" 1" width="88%" />
    </td>
    <td align="center" width="33.33%">
      <strong>缓存大小配置</strong><br />
      <sub>缓存大小配置,LRU自动删除</sub><br /><br />
      <img src="./snap/2.PNG" alt="2" width="88%" />
    </td>
    <td align="center" width="33.33%">
      <strong>缓存管理</strong><br />
      <sub>管理和清除本地缓存</sub><br /><br />
      <img src="./snap/3.PNG" alt="新增截图 3" width="88%" />
    </td>
  </tr>
</table>

## 适用场景

适合用于：

- 个人有声书库的 iPhone 客户端
- 基于 `ting-reader` 后端能力的移动端听书方案
- 有声内容管理、播放与收听体验验证
