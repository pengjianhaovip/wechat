#模块开发的配置


项目结构配置文件: manifest.xml

```xml
<xm<x>l version="1.0" encoding="utf-8"?>
<manifest xm<x>lns="http://www.we7.cc" versionCode="0.6">
    <application setting="true" cloud_setting="true">
        <name><![CDATA[微商城]]></name>
        <identifie><![CDATA[ewei_shopping]]></identifie>
        <version><![CDATA[6.9.9]]></version>
        <type><![CDATA[business]]></type>
        <ability><![CDATA[微商城]]></ability>
        <desc<x>ription><![CDATA[微商城]]></desc<x>ription>
        <author><![CDATA[WeEngine Team & ewei]]></author>
        <url><![CDATA[url]]></url>
    </application>
    <platform>
        <subscribes>
            <message type="text"></message>
            <message type="image"></message>
            <message type="voice"></message>
            <message type="video"></message>
            <message type="shortvideo"></message>
            <message type="location"></message>
            <message type="li<x>nk"/>
            <message type="subscribe"></message>
            <message type="unsubscribe"></message>
            <message type="qr"></message>
            <message type="trace"></message>
            <message type="click"></message>
            <message type="view"></message>
            <message type="merchant_order"></message>
            <message type="user_get_card"></message>
            <message type="user_del_card"></message>
            <message type="user_consume_card"></message>
        </subscribes>
        <handles>
            <message type="text"></message>
            <message type="image"></message>
            <message type="voice"></message>
            <message type="video"></message>
            <message type="shortvideo"></message>
            <message type="location"></message>
            <message type="li<x>nk"/>
            <message type="subscribe"></message>
            <message type="qr"></message>
            <message type="trace"></message>
            <message type="click"></message>
            <message type="merchant_order"></message>
            <message type="user_get_card"></message>
            <message type="user_del_card"></message>
            <message type="user_consume_card"></message>
        </handles>
        <supports>
            <item type="plugin" ></item>
            <item type="wxapp" ></item>
            <item type="app" ></item>
            <item type="system_welcome" ></item>
            <item type="webapp" ></item>
        </supports>
        <plugin-main name="wx_nstore" ></plugin>
        <plugins>
            <item name="ewei_hotel" ></item>
            <item name="ewei_hotel2" ></item>
        </plugins>
        <rule em<x>bed="true" />
        <card em<x>bed="true" />
        <oauth type="userinfo" ></oauth>
    </platform>
    <bindings>
        <cover>
            <entry title="功能封面" do="cover" state="" direct="false"></entry>
            <entry title="功能封面2" do="cover2" state="" direct="false"></entry>
        </cover>
        <rule>
            <entry title="规则" do="rule" state="" direct="false"></entry>
            <entry title="规则2" do="rule2" state="" direct="false"></entry>
        </rule>
        <menu>
            <entry title="管理中心" do="menu" state="" direct="false"></entry>
            <entry title="管理中心2" do="menu2" state="" direct="false"></entry>
        </menu>
        <home>
            <entry title="首页导航" do="home" state="" direct="false"></entry>
            <entry title="首页导航2" do="home2" state="" direct="false"></entry>
        </home>
        <profile>
            <entry title="个人中心导航" do="profile" state="" direct="false"></entry>
            <entry title="个人中心导航2" do="profile2" state="" direct="false"></entry>
        </profile>
        <shortcut>
            <entry title="快捷功能" do="shortcut" state="" direct="false"></entry>
            <entry title="快捷功能2" do="shortcut2" state="" direct="false"></entry>
        </shortcut>
        <function>
            <entry title="独立功能" do="func" state="" direct="false"></entry>
            <entry title="独立功能2" do="func2" state="" direct="false"></entry>
        </function>
        <page>
            <entry title="首页" do="/we7_gs/pages/index/index" state="" direct=""></entry>
            <entry title="主页" do="/we7_gs/pages/index/main" state="" direct=""></entry>
        </page>
        <system_welcome>
            <entry title="systemwelcome" do="systemwelcome" state="" direct="false"></entry>
        </system_welcome>
        <webapp>
            <entry title="webapp" do="webapp" state="" direct="false"></entry>
        </webapp>
    </bindings>
    <permissions>
        <entry title="title1" do="permission1"></entry>
        <entry title="title2" do="permission2"></entry>
    </permissions>
    <install><![CDATA[install.php]]></install>
    <uninstall><![CDATA[uninstall.php]]></uninstall>
    <upgrade><![CDATA[upgrade.php]]></upgrade>
</manifest>


```