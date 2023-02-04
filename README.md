#【特斯拉3.0.0测试包说明】

（1）简繁中文插件整合包基于zdm65477730大佬做的终极版tesla核心，不能兼容各种ovl原版插件，需要由大佬进行适配，目前该插件只能在简体中文或繁体中文系统下正常使用。小弟整合了大佬发布的插件，作为tesla3.0.0测试。

终极版tesla地址：

https://www.tekqart.com/thread-222735-1-1.html

tesla3.0.0有两个问题等大佬更新解决。

1，不可以随意加ovl插件，删减没问题，增加会造成tesla开机奔溃，所以3.0.0删除了2.2插件包中的fastcfwswitch，Triplayer等ovl插件，除非大佬根据终极版核心做对应ovl插件的适配。

2，如果系统语言改成英语、日语等非中文之后会出现tesla死机。

所以默认tesla3.0.0插件包所有插件自动不启动，首次使用，先进相册在Hekate/Deepsea工具箱里Background services中设置Tesla为ON，设置完毕按B退出，再按Home保存后退出，可以启动tesla菜单。

（2）开机出现tesla奔溃死机，可以在重启的时候进Hekate。

有3种方法解决，任选1种。

1，USB工具连PC，删除文件tf：atmosphere/contents/420000000007E51A/flags/boot2.flag，重启。

2，payloads中点Tegraexplorer.bin文件管理器，删除文件tf：atmosphere/contents/420000000007E51A/flags/boot2.flag，重启。

3，payloads中点CommonProblemResolver.bin，第一行disable automatic sysmodule startup，重启。

（3）Tesla插件包更新方法

小弟发布的Tesla插件包只要你之前没添加过其它插件，可以在原插件包上进行覆盖更新，但是3.0.0相当于一个新的插件包，只有2.2可以向2.1和2.0插件包上覆盖。

如果是不同的Tesla插件包的更换，建议删除下面TF卡上旧的3个文件夹后再覆盖

tf：Atmosphere/Contents/

tf：config/

tf：Switch/.overlays/

小弟发布的Tesla插件包有可精简组件说明，大家可以根据说明删除干净每一个插件，或使用文件对比工具Beyond Compare精简。
