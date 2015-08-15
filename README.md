
# 口碑APP UI开发规范

* 旨在规范APP上的视觉元素的使用和与开发的对接，保持风格一致性和可传承，同时提高开发效率
* BRK(brk)表示


-----
## iOS部分
_( `高亮`表示本期修改 )_


### 颜色


#### a.灰度


|ID	|颜色名	|16进制色值	|RGB	|应用示例|
|:--|:--|:--|:--|:--|
|brkColorBlack	|黑色	|#3A3A3A|38，38，38|标题，正文等|
|brkColorGray1	|灰色1	|#666666|102,102,102|列表部分参数|
|brkColorGray2	|灰色2	|#9B9B9B|155,155,155|小标题，附属说明文字|
|brkColorGray3	|灰色3	|#B4B4B5|180,180,181| |
|brkColorGray4	|灰色4	|#D8D8D8|216,216,216|输入框内的提示文字|
|brkColorWhite	|白色	|#FFFFFF|255,255,255|深色背景上文字|


#### b.元素


|ID	|颜色名	|16进制色值	|RGB	|应用示例|
|:--|:--|:--|:--|:--|
|brkColorBgPage	|页面背景色	|#F4F4F5|250,250,250|各页面背景|
|brkColorBgBar	|栏背景色		|#F8F8F9|248,248,249|各种栏的背景色|
|brkColorBgContent	|内容背景色	|#FFFFFF|255,255,255|内容块的背景色|
|brkColorBgSelect	|选中背景色	|#d6d6d6|214,214,214|内容块（卡片，列表）选中色|
|brkColorLine	|分割线色		|#C8C7CC|200,199,204|分割线|
|brkColorOption	|操作色		|#5677FC|86,119,252|操作图标，文字链接的颜色|
|brkColorBgNotice	|通知色	|#FFD578|255,213,120|通知消息|
|brkColorBgWarning	|警告色	|#FF4081|255,64,129|警告消息|


#### c.彩色


|ID	|颜色名	|16进制色值	|RGB	|应用示例|
|:--|:--|:--|:--|:--|
|brkColorBlue			|蓝色(主色调)	|#5677FC|86,119,252|顶栏 |
|brkColorBlueLight		|浅蓝色	|#D0D9FF|208,217,255| |
|brkColorBlueDark		|深蓝色	|#455EDE|69,94,222| |
|brkColorAccent			|高亮色	|#40C4FF|64,196,255|按钮，部分控件 |
|brkColorAccentLight	|浅高亮色	|#80D8FF|128,216,255| |
|brkColorAccentDark		|深高亮色	|#0091EA|0,145,234| |


### 透明度


|ID	|16进制ALPHA值	|百分比100%	|说明|
|:--|:--|:--|:--|
|brkAlpha0	|E6	|90%	||
|brkAlpha1	|B3	|70%	||
|brkAlpha2	|66	|40%	||
|brkAlpha3	|33	|20%	||


### 字体


* iOS中文字体统一为黑体-简(Heiti-SC)，英文字体统一为Helvetica Neue


|ID|字号名|size_@2x(设计)|size(开发)|中文字重(Weight)|英文字重(Weight)|
|:--|:--|:--|:--|:--|:--|
|brkFontDisplay4	|显示4	|144|72	|Light	|Regular|
|brkFontDisplay3	|显示3	|96	|48	|Light	|Regular|
|brkFontDisplay2	|显示2	|72	|36	|Light	|Regular|
|brkFontDisplay1	|显示1	|60	|30	|Light	|Regular|
|brkFontHeadline	|头条	|40	|20	|Light	|Regular|
|brkFontTitle2		|标题2	|34	|17	|Medium	|Medium|
|brkFontTitle1		|标题1	|34	|17	|Light	|Regular|
|brkFontSubhead		|副标题	|30	|15	|Light	|Regular|
|brkFontBody2		|主体2	|28	|14	|Medium	|Medium|
|brkFontBody1		|主体1	|28	|14	|Light	|Regular|
|brkFontCaption		|说明	|24	|12	|Light	|Regular|
|brkFontMenu		|菜单	|30	|15	|Light	|Regular|
|brkFontButton2		|按钮2	|40	|20	|Medium	|Medium|
|brkFontButton1		|按钮1	|40	|20	|Light	|Regular|


### 间距


|ID	|px_@2x(设计)	|点(开发)	|说明|
|:--|:--|:--|:--|
|brkMarginChapter	|64	|32	||
|brkMarginSection	|48	|24	||
|brkMarginPart		|40	|20	||
|brkMargin1			|4	|2	||
|brkMargin2			|8	|4	||
|brkMargin3			|12	|6	||
|brkMargin4			|16	|8	||
|brkMargin5			|20	|10	||
|brkMargin6			|24	|12	||
|brkMargin7			|28	|14	||
|brkMargin8			|32	|16	||
|brkMargin9			|36	|18	||


### 圆角


|ID	|圆角名	|px_@2x(设计)	|dp(开发)	|
|:--|:--|:--|:--|
|brkCircularXLarge	|特大圆角	|30	|15	|
|brkCircularLarge	|大圆角	|16	|8	|
|brkCircularMedium	|中圆角	|8	|4	|
|brkCircularSmall	|小圆角	|4	|2	|


### 命名规则

#### 命名方式：

**`模块名`＋`页面名`＋`图片类型`＋`图片描述`＋`图片状态`**
		
* 图片状态指按下或点击等，正常状态省略


#### 例：		

>**登录模块，注册页面的注册图标：**

>-

>非选中：  	`sign_signin_icon_gosign.png`

>选中：   	`sign_signin_icon_gosign_slt.png`


	
#### 注：


1. 模块名如下：	
	
|命名|对应模块|
|:--|:--|
|_`comm`_	|公用模块|
|_`sign`_	|登录模块|
|_`prop`_	|房源模块|
|_`cstm`_	|客户模块|
|_`sqr`_	|广场模块|
|_`my`_		|我的模块|   


2. 状态名如下：	
	
|命名|对应模块|
|:--|:--|
|_`slt`_	|按下，选中|
|_`dis`_	|不可用|


___

