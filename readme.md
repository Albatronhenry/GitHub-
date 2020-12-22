github，oschina git gitcafe的代码托管平台上的项目的Readme.MD文件都是有其特有的语法的,基本规则如下：

问题：raw.githubusercontent.com github的raw文件访问不了

简单的说就是域名被DNS污染了

在C:\Windows\System32\drivers\etc下的hosts文件加上：199.232.4.133 raw.githubusercontent.com

[html] view plain copy
Markdown 语法速查表  
1 标题与文字格式  
标题  
# 这是 H1 <一级标题>  
## 这是 H2 <二级标题>  
###### 这是 H6 <六级标题>  
文字格式  
**这是文字粗体格式**  
*这是文字斜体格式*  
~~在文字上添加删除线~~  
2 列表  
无序列表  
* 项目1  
* 项目2  
* 项目3  
有序列表  
1. 项目1  
2. 项目2  
3. 项目3  
   * 项目1  
   * 项目2  
3 其它  
图片  
![用友政务](http://www.yonyougov.com/statics/images/logo.png)  
链接  
[用友政务](http://www.yonyougov.com/)  
引用  
> 第一行引用文字  
> 第二行引用文字  
水平线  
***  
代码  
`<hello world>`  
代码块高亮  
```ruby  
  def add(a, b)  
    return a + b  
  end  
```  

部分文字的高亮
如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，那么可以把它用 `  ` 包围起来。注意这不是单引号，而是Tab上方，数字1左边的按键（注意使用英文输入法）。

Thank `You` . Please `Call` Me `Coder`


表格  
  表头  | 表头  
  ------------- | -------------  
 单元格内容  | 单元格内容  
 单元格内容l  | 单元格内容  
 
 
 | Item     | Value | Qty   |
| :-------  | ----: | :---: |
| yonyougov | $1600 |  10   |
| ufgov     | $1800 |  12   |
| yonyou    | $2000 |  23   |


>数据结构  
>>树  
>>>二叉树  
>>>>平衡二叉树  
>>>>>满二叉树  

表情
Github的Markdown语法支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如:blush:，可以显示:blush:。

具体每一个表情的符号码，可以查询GitHub的官方网页http://www.emoji-cheat-sheet.com。

但是这个网页每次都打开奇慢。。所以我整理到了本repo中，大家可以直接在此查看emoji。

如果直接记语法，那似乎困难了些。这里OneCoder推荐两个Markdown的编辑器。

在线编辑器：stackedit
网址：https://stackedit.io/

Mac下离线编辑器Mou
下载地址：http://mouapp.com/


OneCoder这里使用的是后者为自己的shurnim-storage项目写Readme。至于这个项目是什么，见Readme文档，OneCoder也会在另外的博文做一些补充说明。成品Readme如下：

[html] view plain copy
# Albatronhenry  
  
![yonyougov icon](http://www.yonyougov.com/statics/images/logo.png)  


  
## 目录  
* [背景介绍](#背景介绍)  
* [项目介绍](#项目介绍)  
* [使用说明](#使用说明)  
  * [获取代码](#获取代码)  
  * [开发插件](#开发插件)  
  * [使用ShurnimStorage接口](#使用ShurnimStorage接口)  
       * [接口介绍](#接口介绍)  
       * [使用样例](#使用样例)  
* [其他](#其他)  
  
<a name="背景介绍"></a>  
## 背景介绍  
  
*Ahenry*<br/>  
*A++*，代表Advance+Application，表示领先、应用的意思。  
  
<a name="携手发力管理信息化 联袂深耕大数据分析 中国科学院与用友政务共同创立“管理大数据研究院”"></a>  
## 项目介绍  
  
### 随着大数据、“互联网+政务服务”上升为国家战略，信息技术正在渗透到政府及公共事业管理的各个方面，给政府及公共事业管理带来一场新的革命。

8月29日，中国科学院计算机网络信息中心与用友集团旗下的北京用友政务软件有限公司宣布共同创立“管理大数据研究院”，推进在管理信息化和大数据分析领域的前沿技术研发和战略合作。

借此契机，双方将充分发挥各自优势，以基于财税、财务和资产管理等方面的大数据分析挖掘为核心，以攻关复杂科研项目管理模式为导向，联合开展用户行为分析、深度学习、管理态势等关键技术攻关，促使双方在管理信息化和管理大数据治理等领域拥有国内领先、国际一流的技术优势，推进科技成果转移转化。


“这是一项具有引领创新作用的战略性举措，对建设‘智慧中科院’和打造‘用友云’都有十分重要的现实意义。”中国科学院网信办副主任陈明奇首先在签约仪式上对战略合作提出几点希望：一是进一步明确定位和方向。做到一个引领、两个接轨、三个能力。一个引领即：在管理信息化领域形成国内领先的技术优势，领跑业界发展。两个接轨即：与国家治理体系现代化接轨和与新一代信息技术发展趋势接轨。三个能力即：管理业务与信息技术的融合能力、系统平台与数据应用的集成能力、成果转化与培养市场的拓展能力。二是进一步聚焦产品实践。三是贡献管理信息化的“中科院方案”。

用友领航企业软件与信息化服务30年，致力于成为全球领先的企业服务提供商，已经走过了1.0用友财务软件时期，2.0用友ERP时期，现在已经进入到用友3.0发展时期，形成了以用友云为核心的企业服务，致力于推动企业和公共组织互联网化、金融化创新发展，服务IT产业转型升级。用友云定位社会化商业应用基础设施及企业服务产业的共享平台，用友云通过各项云服务帮助企业客户 “敏经营、轻管理、易金融、简IT”，赋能中国企业，最终实现增长收入、降低成本、提高效率和控制风险。



据了解，为了确保用友云在政府行业落地并保持领先，用友政务公司将 “大数据”和“政务云”列入重要战略规划，在综合治税、精准扶贫、社会保障资金使用效益、地方政府债务分析与预警、反不正当支付、财政供养、企业扶持等层面做着积极的努力和实践，而且已经有了很多成熟的产品和案例。




此次战略合作体现了双方领导运用创新驱动发展的战略思维，是国立科研机构与大型创新企业合作的一次有益尝试。中国科学院计算机网络信息中心管理信息化部主任焦文彬介绍道，中国科学院的管理信息化平台，也就是ARP系统已经运行了十余年。当前，以“大、智、物、移、云”为特征的新一代信息技术的应用已经全面展开，大数据环境正在快速形成。中国科学院的ARP发展与企业ERP发展面临着同样的困局。如何运用大数据优势实现管理工作的智慧化和决策依据的科学化，运用新一代信息技术实现管理软件的升级换代，是我们都需要面对的严峻挑战。当然，其中也蕴藏着巨大的机遇。“中国科学院计算机网络信息中心正在按照院里‘十三五信息化规划’的要求，着力打造新一代ARP。当前面临的机遇与挑战为双方合作提供了坚实的基础。”
  
<a name="使用说明"></a>  
## 使用说明  
  
<a name="获取代码"></a>  
### 获取代码  
  
* 主页: <https://github.com/Albatronhenry/>  
* 主页: <https://github.com/Albatronhenry/><br>  
  
OSChina的Maven库获取依赖，或者自己编译jar包。  
  
* maven  
  
     1. 加入OSC仓库  
     
                    <repositories>  
                      <repository>  
                           <id>nexus</id>  
                           <name>local private nexus</name>  
                           <url>http://maven.oschina.net/content/groups/public/</url>  
                           <releases>  
                                <enabled>true</enabled>  
                           </releases>  
                           <snapshots>  
                                <enabled>false</enabled>  
                           </snapshots>  
                      </repository>  
                 </repositories>  
  
     2. 加入依赖  
     
               <dependency>  
                 <groupId>com.coderli</groupId>  
                 <artifactId>shurnim-storage</artifactId>  
                  <version>0.1-alpha</version>  
               </dependency>  
* Gradle 编译Jar  
  
在项目目录执行  
     
     gradle jar  
     
<a name="开发插件"></a>  
### 开发插件  
  
在*shurnim-storage*中，插件就像一块一块的积木，不但支撑着框架的功能，也是框架可扩展性的基石。开发一个插件，仅需两步：  
  
1. 实现PluginAPI接口  
  
```  
package com.coderli.shurnim.storage.plugin;  
  
import java.io.File;  
import java.util.List;  
  
import com.coderli.shurnim.storage.plugin.model.Resource;  
  
/**  
* 各种云存储插件需要实现的通用接口  
*/  
public interface PluginAPI {  
  
     /**  
      * 初始化接口  
      */  
     void init();  
  
     /**  
      * 获取子资源列表  
      *  
      * @param parentPath  
      */  
     List<Resource> getChildResources(String parentPath);  
  
     /**  
      * 下载特定的资源  
      *  
      * @param parentPath  
      *            目录路径  
      * @param name  
      *            资源名称  
      * @param storePath  
      *            下载资源保存路径  
      * @return  
      */  
     Resource downloadResource(String parentPath, String name, String storePath);  
  
     /**  
      * 创建文件夹  
      *  
      * @param path  
      *            文件夹路径  
      * @param auto  
      *            是否自动创建父目录  
      * @return  
      */  
     boolean mkdir(String path, boolean auto);  
  
     /**  
      * 上传资源  
      *  
      * @param parentPath  
      *            父目录路径  
      * @param name  
      *            资源名称  
      * @param uploadFile  
      *            待上传的本地文件  
      * @return  
      */  
     boolean uploadResource(String parentPath, String name, File uploadFile);  
}  
```  
  
目前插件的接口列表仅为同步资源设计，如果想要支持更多操作(如删除，查找等)，可扩展该接口定义。<br/><br/>  
接口中，所有的参数和返回值均为*shurnim-storage*框架中定义的通用模型。因此，您在开发插件过程中需要将特定SDK中的模型转换成接口中提供的模型。<br/><br/>  
插件实现类只要与*shurnim-storage*工程在同一个classpath即可使用。您既可以直接在源码工程中开发插件，就如工程里提供的*upyun*和*qiniu*插件一样，也可以作为独立工程开发，打成jar，放置在同一个classpath下。<br/><br/>  
*upyun*插件样例(功能不完整):  
  
```    
package com.coderli.shurnim.storage.upyun.plugin;  
  
import java.io.File;  
import java.util.List;  
  
import com.coderli.shurnim.storage.plugin.AbstractPluginAPI;  
import com.coderli.shurnim.storage.plugin.model.Resource;  
import com.coderli.shurnim.storage.plugin.model.Resource.Type;  
import com.coderli.shurnim.storage.upyun.api.UpYun;  
  
public class UpYunPlugin extends AbstractPluginAPI {  
  
     private UpYun upyun;  
     private String username;  
     private String password;  
     private String bucketName;  
  
     public UpYun getUpyun() {  
          return upyun;  
     }  
  
     public void setUpyun(UpYun upyun) {  
          this.upyun = upyun;  
     }  
  
     public String getUsername() {  
          return username;  
     }  
  
     public void setUsername(String username) {  
          this.username = username;  
     }  
  
     public String getPassword() {  
          return password;  
     }  
  
     public void setPassword(String password) {  
          this.password = password;  
     }  
  
     public String getBucketName() {  
          return bucketName;  
     }  
  
     public void setBucketName(String bucketName) {  
          this.bucketName = bucketName;  
     }  
  
     /*  
      * (non-Javadoc)  
      *  
      * @see  
      * com.coderli.shurnim.storage.plugin.PluginAPI#getChildResources(java.lang  
      * .String)  
      */  
     @Override  
     public List<Resource> getChildResources(String parentPath) {  
          return null;  
     }  
  
     /*  
      * (non-Javadoc)  
      *  
      * @see  
      * com.coderli.shurnim.storage.plugin.PluginAPI#downloadResource(java.lang  
      * .String, java.lang.String, java.lang.String)  
      */  
     @Override  
     public Resource downloadResource(String parentPath, String name,  
               String storePath) {  
          File storeFile = new File(storePath);  
//          if (!storeFile.exists()) {  
//               try {  
//                    storeFile.createNewFile();  
//               } catch (IOException e) {  
//                    e.printStackTrace();  
//               }  
//          }  
          String filePath = getFullPath(parentPath, name);  
          upyun.readDir("/api");  
          if (upyun.readFile(filePath, storeFile)) {  
               Resource result = new Resource();  
               result.setName(name);  
               result.setPath(parentPath);  
               result.setType(Type.FILE);  
               result.setLocalFile(storeFile);  
               return result;  
          }  
          return null;  
     }  
  
     String getFullPath(String parentPath, String name) {  
          if (!parentPath.endsWith(File.separator)) {  
               parentPath = parentPath + File.separator;  
          }  
          return parentPath + name;  
     }  
  
     /*  
      * (non-Javadoc)  
      */  
     @Override  
     public boolean mkdir(String path, boolean auto) {  
          // TODO Auto-generated method stub  
          return false;  
     }  
  
     /*  
      * (non-Javadoc)  
      *  
      * @see  
      * com.coderli.shurnim.storage.plugin.PluginAPI#uploadResource(java.lang  
      * .String, java.lang.String, java.io.File)  
      */  
     @Override  
     public boolean uploadResource(String parentPath, String name,  
               File uploadFile) {  
          // TODO Auto-generated method stub  
          return false;  
     }  
  
     /*  
      * (non-Javadoc)  
      *  
      * @see com.coderli.shurnim.storage.plugin.AbstractPluginAPI#init()  
      */  
     @Override  
     public void init() {  
          upyun = new UpYun(bucketName, username, password);  
     }  
  
}  
```  
  
  
2. 编写插件配置文件  
  
```  
<?xml version="1.0" encoding="UTF-8"?>  
<plugin>  
     <id>henry</id>  
     <name>Alabatron</name>
     <api>  
          <className>com.coderli.shurnim.storage.qiniu.QiniuPlugin</className>  
          <params>  
               <param name="access_key" displayName="ACCESS_KEY">EjREKHI_GFXbQzyrKdVhhXrIRyj3fRC1s9UmZPZO  
               </param>  
               <param name="secret_key" displayName="SECRET_KEY">88NofFWUvkfJ6T6rGRxlDSZOQxWkIxY2IsFIXJLX  
               </param>  
               <param name="bucketName" displayName="空间名">onecoder  
               </param>  
          </params>  
     </api>  
</plugin>  
```  
   * **id** 为该插件在*shurnim-storage*框架下的唯一标识，不可重复，必填。  
    * **name** 为显示值，为UI开发提供可供显示的有语义的值。  
    * **className** 为插件接口实现类的完整路径。必填  
    * **params/param** 为插件需要用户配置的参数列表。其中  
         * *name* 代表参数名，需要与接口实现类中的参数名严格一致，且必须有相应的set方法的格式要求严格，即set+首字母大写的参数名。例如:setAccess_key(String arg); 目前只支持*String*类型的参数。  
         * *displayName* 为参数显示名，同样是为了UI开发的考虑，方便用户开发出可根据参数列表动态显示的UI界面。  
         * 参数的值可以直接配置在配置文件中，也可以在运行期动态赋值。直接配置值，对于直接使用后端接口来说较为方便。对于UI开发来说，运行期动态赋值更为合理。<br/></br>  
  
     在使用源码工程时，插件配置文件统一放置在工程的*plugins*目录下。你也可以统一放置在任何位置。此时，在构造后端接口实例时，需要告知接口该位置。  
     
<a name="使用ShurnimStorage接口"></a>  
### 使用*ShurnimStorage*接口  
  
<a name="接口介绍"></a>  
#### 接口介绍  
  
**ShurnimStorage**接口是*shurinm-storage*框架全局的也是唯一的接口，目前定义如  
  
```  
package com.coderli.shurnim.storage;  
  
import java.util.List;  
import java.util.Map;  
  
import com.coderli.shurnim.storage.plugin.model.Plugin;  
import com.coderli.shurnim.storage.plugin.model.Resource;  
  
/**  
* 后台模块的全局接口<br>  
* 通过该接口使用后台的全部功能。<br>  
* 使用方式:<br>  
* <li>  
* 1.先通过{@link #getSupportedPlugins()}方法获取所有支持的平台/插件列表。 <li>  
* 2.将列表中返回的ID传入对应的接口参数中，进行对应的平台的相关操作。<br>  
* 需要注意的是，不同平台的插件需要给不同的参数赋值，该值可以直接配置在配置文件中。<br>  
* 也可以在运行期动态赋值。(会覆盖配置文件中的值。)<br>  
*  
* 参数列表的设计，方便UI开发人员动态的根据参数列表生成可填写的控件。并给参数赋值。增强了可扩展性。  
*  
*/  
public interface ShurnimStorage {  
  
     /**  
      * 获取当前支持的插件列表<br>  
      * 没有支持的插件的时候可能返回null  
      *  
      * @return  
      * @author henry  
      * @date 
      */  
     List<Plugin> getSupportedPlugins();  
  
     /**  
      * 给指定的插件的对应参数赋值<br>  
      * 此处赋值会覆盖配置文件中的默认值  
      *  
      * @param pluginId  
      *            插件ID  
      * @param paramsKV  
      *            参数键值对  
      */  
     void setParamValues(String pluginId, Map<String, String> paramsKV);  
  
     /**  
      * 获取插件对应目录下的资源列表  
      *  
      * @param pluginId  
      *            插件ID  
      * @param path  
      *            指定路径  
      * @return  
      * @author OneCoder  
      * @date 
      */  
     List<Resource> getResources(String pluginId, String path);  
  
     /**  
      * 同步资源  
      *  
      * @param fromPluginId  
      *            待同步的插件Id  
      * @param toPluginIds  
      *            目标插件Id  
      * @param resource  
      *            待同步的资源  
      * @return 同步结果  
      * @author OneCoder  
      * @date 
      */  
     boolean sycnResource(String fromPluginId, String toPluginId,  
                    Resource resource) throws Exception;  
}  
```      
  
当前接口实际仅包含了获取资源列表*getResources*和同步资源*sycnResource*功能，*getSupportedPlugins*和*setParamValues*实际为辅助接口，在UI开发时较为有用。<br/><br/>  
同样，您也可以扩展开发该接口增加更多的您喜欢的特性。例如，同时删除给定存储上的文件。当然，这需要插件接口的配合支持。<br/><br/>  
  
这里，*sycnResource*设计成插件间一对一的形式，是考虑到获取同步是否成功的结果的需求。如果您想开发一次同步到多个存储的功能，建议您重新开发您自己的接口实现类，因为默认实现会多次下次资源(每次同步后删除)，造成网络资源的浪费。  
  
接口的默认实现类是: **DefaultShurnimStorageImpl**  
  
<a name="使用样例"></a>  
#### 使用样例  
```        
package com.coderli.shurnim.test.shurnimstorage;  
  
import org.junit.Assert;  
import org.junit.BeforeClass;  
import org.junit.Test;  
  
import com.coderli.shurnim.storage.DefaultShurnimStorageImpl;  
import com.coderli.shurnim.storage.ShurnimStorage;  
import com.coderli.shurnim.storage.plugin.model.Resource;  
import com.coderli.shurnim.storage.plugin.model.Resource.Type;  
  
/**  
* 全局接口测试类<br>  
* 时间有限，目前仅作整体接口测试。细粒度的单元测试，随开发补充。  
*  
*/  
public class ShurnimStorageTest {  
  
     private static ShurnimStorage shurnim;  
  
     @BeforeClass  
     public static void init() {  
          shurnim = new DefaultShurnimStorageImpl(  
                    "/Users/apple/git/shurnim-storage-for-UPYUN/plugins");  
     }  
  
     @Test  
     public void testSycnResource() {  
          Resource syncResource = new Resource();  
          syncResource.setPath("/api");  
          syncResource.setName("api.html");  
          syncResource.setType(Type.FILE);  
          try {  
               Assert.assertTrue(shurnim.sycnResource("upyun", "qiniu",  
                         syncResource));  
          } catch (Exception e) {  
               e.printStackTrace();  
          }  
     }  
}  
```  
<a name="其他"></a>  
## 其他  
  
* Email: <mr.lin1994@foxmail.com>  
* Blog:[Albatron](https://github.com/Albatronhenry/)  
  


(Reference website1)[http://blog.csdn.net/fenglailea/article/details/45562855]
(Reference website2)[http://www.coderli.com/write-readme-for-your-project/]
