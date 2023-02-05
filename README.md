# 大气层特斯拉3.1.0简繁中文插件整合包-YuanBanban

zdm65477730大佬于2023年2月5日更新switch/.overlays/ovlmenu.ovl文件，解决了tesla3.0.0非中文系统语言导致Tesla奔溃的错误，但是修复后Tesla菜单插件名称只能显示英文，进各个ovl插件不受影响，依然中英文适配。3.1.0插件包新加了两种ovlmenu.ovl，但是默认Switch/.overlays/ovlmenu.ovl是只适配简繁中文系统语言的ovlmenu.ovl。

3.1.0插件包可以直接覆盖到3.0.0插件包升级

（1）适配多国系统语言的ovlmenu.ovl

tf：Switch/.overlays/ovlmenuEN/ovlmenu.ovl，把它覆盖到tf：Switch/.overlays/ovlmenu.ovl，系统语言可以设定中、英、日、法等不受限制，Tesla菜单插件名称只能显示英文。

（2）只适配简繁中文系统语言的ovlmenu.ovl

tf：Switch/.overlays/ovlmenuCN/ovlmenu.ovl，把它覆盖到tf：Switch/.overlays/ovlmenu.ovl，系统语言必须是简体或繁体中文，Tesla菜单插件名称能显示简繁中文。

更换覆盖ovlmenu.ovl文件，既可以通过Hekate的USB工具，DBI的MTP，也可以在nxshell等文件管理器中操作。

# 【特斯拉3.1.0测试包说明】

（1）简繁中文插件整合包基于zdm65477730大佬做的终极版tesla核心，不能兼容各种ovl原版插件，需要由大佬进行适配，目前该插件只能在简体中文或繁体中文系统下正常使用。小弟整合了大佬发布的插件，作为tesla3.0.0测试。

终极版tesla地址：

https://www.tekqart.com/thread-222735-1-1.html

tesla3.1.0插件包不可以随意加ovl插件，删减没问题，增加会造成tesla开机奔溃，所以3.0.0删除了2.2插件包中的fastcfwswitch，Triplayer等ovl插件，除非大佬根据终极版核心做对应ovl插件的适配。

所以默认tesla3.0.0插件包所有插件自动不启动，首次使用，先进相册在Hekate/Deepsea工具箱里Background services中设置Tesla为ON，设置完毕按B退出，再按Home保存后退出，可以启动tesla菜单。

（2）开机出现tesla奔溃死机，可以在重启的时候进Hekate。

有3种方法解决，任选1种。

1，USB工具连PC，删除文件tf：atmosphere/contents/420000000007E51A/flags/boot2.flag，重启。

2，payloads中点Tegraexplorer.bin文件管理器，删除文件tf：atmosphere/contents/420000000007E51A/flags/boot2.flag，重启。

3，payloads中点CommonProblemResolver.bin，第一行disable automatic sysmodule startup，重启。

（3）Tesla插件包更新方法

小弟发布的Tesla插件包只要你之前没添加过其它插件，可以在原插件包上进行覆盖更新，但是3.0.0相当于一个新的插件包，只有2.2可以向2.1和2.0插件包上覆盖。如果是不同的Tesla插件包的更换，建议删除下面TF卡上旧的3个文件夹后再覆盖

tf：Atmosphere/Contents/

tf：config/

tf：Switch/.overlays/

小弟发布的Tesla插件包有可精简组件说明，大家可以根据说明删除干净每一个插件，或使用文件对比工具Beyond Compare精简。

（4）整合大气层就像搭积木，大气层增强包=大气层迷你包+特斯拉插件包+相册NRO软件包，迷你包是必须的，另两个包非必需，整合的时候三个包的版本不用完全对应，都是向下兼容，只要插件包和软件包都能支持大气层或SW系统版本就可以了。

（5）tesla插件有3类

第1类是原版核心的Tesla加载器和Tesla界面，原版核心的优点是兼容不同发布者发布的ovl插件，原版只有英文，所以有不同大佬的汉化，但是汉化有个缺点，会在非简体中文的SW系统中字体缺失，只有英文插件可以无视SW系统语言。除非该插件自带多国语言，比如emuiibo原版插件自带多国语言，并兼容原版tesla核心。

第2类是zdm65477730大佬发布的中英文tesla，基于原版核心，兼容各种ovl插件，并提供edizon，ReverseNX-RT，StatusMonitor，sys-clk等插件的中英文自适配。这也是小弟整合tesla2.0/2.1/2.2插件包的核心。由于大佬已不再基于原版核心开发，所以虽然其它的原版插件都可以随便添加，但只能显示英文。

第3类是zdm65477730大佬做的终极版tesla核心，不能兼容各种ovl原版插件，需要由大佬进行适配，目前该插件只能在简体中文或繁体中文系统下正常使用。小弟整合了大佬发布的插件，作为tesla3.0.0测试版。

# 【插件版本】

3.0.0插件版本为2023.2.4更新，只有missioncontrol-v0.8.0原版和sys-con-v0.6.4原版两个插件不带ovl文件，可以使用原版。

3.1.0插件版本为2023.2.5更新，仅新加适配多国系统语言的ovlmenu.ovl。

