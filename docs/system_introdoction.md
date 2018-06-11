
[TOC]

# <span id="system_introdoction">FlyThings系统介绍</span>
本系统基于Linux系统开发，以MiniGUI为绘图引擎，加入了自主开发的系统框架和GUI交互系统。
我们称之为FlyThings系统。
寓意为：物联网添加一个飞翔的能力

## 系统目标场景：
当前物联网行业发展迅速，液晶显示的发展中国的水平也不断提高并且已经进入了世界领先的地位了。随着液晶显示价格的下降，用户视窗展示的需求，screening正在到来。所有的展示都将变成显示屏。
	中科世为针对目前的发展，提出了目前阶段更加适合的显示解决方案。
    1. 替换Android在一下小应用场景下的使用，比如家电，门禁等功能简单，系统稳定性要求高，性价比要求高的产品场景
    2. 替换传统的黑白显示或者MCU驱动的彩色显示方案，用低成本的方式提高交互体验性。
    3. 物联网和共享场景的到来，带来了更多展示视窗和交互的需求。提供高性价比，高稳定性的系统支持。
    
## 系统的组成
* 内核
	* 基于开源的Liunx3.4的内核版本
	* 针对物联网行业裁剪优化
* 系统
	* 自主的GUI框架
	*  网络API
	*  多媒体服务
	*  物联网平台接入
	*  支付平台接入能力
	*  远程更新系统能力
	*  远程推送消息的能力
* 开发支持
	* 提供所见即所得组态式GUI开发工具
	* 提供完整的逻辑代码开放编写部分
	* 不断更新的文档和样例支持
	* 不断更新的控件包和系统升级服务