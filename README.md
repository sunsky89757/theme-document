😁作为一个程序员，在日常的工作、生活、学习的过程中基本都有很多需要做笔记的地方；做笔记的主要目的之一是为了“温故而知新”，另一个则是为了在下一次遇到的时候，不需要再次耗费精力去找解决方法；

回顾自己之前写的那个主题，不管是写还是查都不怎么方便，最终下定决心重写一个主题；以 “方便记、方便查、简约”作为设计核心；

本文则记录主题从诞生至今所有的开发记录；
# 2022-06-03
端午节，在style.css里敲下了第一段代码，描述主题。🤣然后初步确定主要需要具备的一些功能：
```
/*
Theme Name: Document
Theme URI: https://nicen.cn
Author: 友人a丶
Author URI: https://nicen.cn
Description: 一个基于文档类型的博客主题，更加方便的记录、查询学习笔记
Version: 1.0
License: GNU General Public License v2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Text Domain: Document
Tags: 文档,自适应,主题切换,阅读进度跟随
*/
```
## 1.文章目录导航
能够根据文章内容自动生成文章目录，虽然这个前端实现比较方便，但是考虑到需要seo所以直接在后端生成；

文章目录导航需要自动跟随阅读进度，点击文章目录导致自动跳转到对应的内容；

文章目录最小高度为屏幕的一半，悬浮在文章左侧；

## 2. 黑夜、白天阅读模式切换、主题色切换
   支持黑夜、白天阅读模式，主题色切换，悬浮在屏幕右下角，附带一个屏幕滚动进度；

## 3. 主题前端元素
1. 代码高亮
2. 代码块一键复制
3. 成功文字块、失败文字块、警告文字块
4. 文字标记
5. 图片灯箱
6. 一级、二级、三级标题
7. 作者信息卡片
8. 文章信息卡片
9. 评论区
10 最新文章
11. 文章导航
12. 文章底部赞赏
13. 站点底部信息
14. 导航栏菜单
15. 导航栏搜索
16. 上一篇、下一篇文章
17. 一键回到顶部
18. 主题色、阅读模式切换
19. 文章点赞、踩
20. 文章浏览、评论、发布时间、作者信息显示
    
## 主题前端优化
   1. 文章页右边栏正常高度时，跟随文章滚动，滚动高度超出侧边栏高度时自动悬浮，保持右边侧边栏始终存在元素，不会空白；
   2. 访问首页时显示自定义的站点描述，文章页时自动截取文章内容作为网页描述；
   3. 优化Gavatar头像，改为国内镜像服务器；
## 主题后端优化
   1. 自动切换到经典编辑器。
   2. 去除后台加载的无用代码。
   3. 增加后台设置，可设置主题的基本信息：关键词、主题描述、作者信息等；
   4. 增加编辑器插件：代码高亮、一级、二级、三级标题、成功文字块、错误文字块、失败文字块、图片灯箱、文字标记
   5. 新增元标签：一级、二级、三级标题、成功文字块、错误文字块、失败文字块、图片灯箱、文字标记
   6. 自定义顶部菜单
   7. 404页面
   8. 搜索空结果页面
   9. 文章密码权限控制
