## ǰ��

���ǵ�����һ�죬�������Ƶؾͽ�����ĳè�������㶮�ģ����Ӵˣ�ÿ������һƿӪ�����ߡ����ҵ��ǣ�������Ϊ��ӯ����������VIPͨ���Ͳ��Ŵ������ƣ���Ȼ����ֱ�Ӻȵ������ˡ�������ֵ�ഺ��������ʢ�����ǣ���ô�������ǿ����������Ǿͳ�Ϊ�ߴ��ϵĻ�Ա������VIP����ͨ�������޹ۿ�����Ǯ����Ǯ�ǲ����ܳ�Ǯ�ģ��Ⱳ�Ӷ������ܳ�Ǯ����ΪAndroid�����ߣ�Ӧ����������ֶ����㶨��������飬��������Ŀ�꣬�Ǿ���һ��Android������֮�ðɣ�    

�������ĵ�Ŀ�ģ����˷��������ƽ�����⣬��ϣ�����԰������Android����Ĵ��ţ����鲻һ����Android���硣
    
...ûʱ������ˣ��Ͻ��ϳ���..

## ׼������

������Ļ������ߣ�������Ҫ׼��Android���������� **[apktool](https://ibotpeaches.github.io/Apktool/)**��**[dex2jar](https://sourceforge.net/projects/dex2jar/)**��**[jd-gui](http://java-decompiler.github.io/)**

apktool��������apk�����´����apk������Եõ� **smali��res��AndroidManifest.xml** ���ļ���

dex2jar����Androidִ�е� **dex** �ļ�ת�� **jar** �ļ���

jd-gui��һ����Է����Ķ� **jar** �ļ��Ĵ��빤�ߡ�

����֮��Ĺ�ϵ�����Բο���ͼ��

<img src="https://user-gold-cdn.xitu.io/2019/8/9/16c7599d4ee4648d?w=690&h=411&f=jpeg&s=39307" />

> ���غ������������ߣ��Ϳ��Կ����������֮���ˣ�

## ����ʼ

> �ᵽ���򣬿��ܺܶ����ѻ��뵽Xposed����XposedȥHook�������ƹ�if�жϡ�û����Xposedȷʵ�����׾��ܴﵽĿ�ģ������������ƱȽϴ��ֻ���Ҫroot�����Ұ�װXposedģ�飬������Ҫ����VirtualXposed���⻷���£�������ʹ���ߵ����ֳɱ���

����������ƽⷽʽ����ֱ�����һ���ƽ��Apk��ʹ���߲���Ҫ�����κζ���Ĳ�������װ����ʹ�á�

### ��һ������ԭӦ�� apk ��׺�ĳ� zip����ѹ�� classes.dex �ļ�

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7b6669657559d?w=172&h=106&f=png&s=8524" />

</br>

<img src="https://user-gold-cdn.xitu.io/2019/8/9/16c75c62807636e9?w=660&h=367&f=png&s=21694" width="440" hegiht="244" align=center />
    
> ��ʵ��һ�������ѵģ��������ѵ������ѿǣ��ѿǷ����֣��ֶ��ѿ�(����)�ͻ����ѿ�(����)��ʲô���ѿ��أ����Ǻܶ�App�ڷ�����Ӧ���г�֮ǰ������мӹ̣����ӿǣ������������dex�ļ���"��"���������Ǿ���Ҫͨ���ѿǵķ�ʽȥ�ҵ�Ӧ����������dex�������õ������Դ�롣ֻ���õ�Դ�벢����Դ��(���������ɴ���)�������ҵ����Ƶ㣬�����޸Ĵ������±��롣

>���������ƽ��ĳèApp����Ϊ�����������ʣ����ϲ����г���Ҳû�мӹ̣���������ǣ�����Ȼ�����������������ƽ���Ѷ�ֱ���½���
    
### �ڶ�����ʹ�� dex2jar �� classes.dex ת�� jar �ļ�
 
 cmd��dex2jar�ļ���Ŀ¼��ִ��
 
```cmd
    d2j-dex2jar D://xxx/xxx/classes.dex
```

�õ� **jar** �ļ�

<img src="https://user-gold-cdn.xitu.io/2019/8/9/16c75d87edd7ef60?w=596&h=28&f=png&s=2572" width="596" hegiht="28" align=center />

### ���������� jar �ļ��� jd-gui �򿪣��鿴Դ����

<img src="https://user-gold-cdn.xitu.io/2019/8/9/16c75daa65e3f220?w=875&h=635&f=png&s=91460" width="437" hegiht="317" align=center />

## ��̬����

�õ�Դ�������������Ҫ�ҵ�Ӧ�õ����Ƶ㣬�ƹ�App������жϡ�

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7b7bb608c1837?w=540&h=960&f=jpeg&s=22805" width="270" hegiht="480" align=center />

Ȼ�����Դ�룬�ô����￪ʼ�����أ�

���Ƕ�֪����һ������AndroidӦ�ã����ܻ���ڸ��ֵ����������������⣬��Щ�������ᱻ���뵽dex���棬�������Jar���������ںܶ಻ͬ���������ļ���Ϊ�˷����ҵ��ƽ�Ӧ�õİ��������ǿ��Խ���adb��ӡջ��activity����ȫ·����

```cmd
    adb shell dumpsys activity | findstr "mFocusedActivity"
```

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7b8b4b0b58291?w=673&h=261&f=png&s=27446"/>

activity�İ�·���Ѿ���ӡ�����ˣ��������� jar �ļ������ҵ� **PlayLineActivity.java** ����ش��롣

����ҳ��Toast��ʾ�������ɾ��ܶ�λ�����Ƶ㡣

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7b8e55ce67c75?w=837&h=516&f=png&s=81619"/>

```java
    UserUtils.getUserInfo().getIs_vip().equals("1")
```

���Կ���������Ա�ֶ�Ϊ 1 ʱ��˵���ǻ�Ա�û����ͻ��л�����·2��

```java
    Hawk.put("line", "2");
```

�ǽ�����ֻ��Ҫ�޸��û�ʵ���� **UserModel** �� **getIs_vip()** ������������Զ���� **1** �����ˡ�

## �ƽ�

**dex2jar��jd-gui** ��ֻ�Ƿ������ߣ�������������ƽ�Ŀ�ʼ��

### Smali���

> Dalvik�������Jvmһ����Ҳ���Լ���һ��ָ������ƻ�����ԣ����ǱȻ�����ࡣ���Ǳ�д��Java�࣬��󶼻�ͨ�������ת����Androidϵͳ���Խ����smaliָ����ɺ�׺Ϊ .smali ���ļ�����Java�ļ�һһ��Ӧ��Ҳ���ܻ��Java�ļ��࣬���͵ı���ʵ��ĳ���ӿڵ������ڲ��ࣩ����Щsmali�ļ�����Dalvik�ļĴ������ԡ� ֻҪ���java���˽�android�����֪ʶ���������ɵ��Ķ�����

���ԣ�����������Ҫ�޸ĵĶ������� java �����Ӧ�� smali ָ�

### ������

��������apktool���ߣ�����ȡapk����� smali�ļ���

cmd��apktool�ļ������棬ִ�� ����Ҳ�������û��������������᷽��һЩ��

```cmd
    apktool.bat d -f [apk����·��] [�ļ������·��]
```

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bacf87ce677b?w=697&h=110&f=png&s=16031"/>

������ɹ��󣬴�smali�ļ��У��ҵ� **UserModel.java** ��Ӧ�����µ� **UserModel.smali** �ļ���

### ����

�ҵ��˱����ļ����ҵ��˱��Ƶ㣬�������Ϳ��Զ� **UserModel.smali** �ļ����б����ˣ�Ϊʲô�б��ƣ���Ҳ��֪�������ڶ��������еģ��о��ߴ��ϣ���ʵ�����޸��ļ�����

�ñ༭���� **UserModel.smali** ���ҵ� **getIs_vip** ����

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bb829aa1eb38?w=988&h=220&f=png&s=16335"/>

���Կ������������˳�Ա���� **is_vip** ��ֵ������ֻ��Ҫ�����ķ���ֵ�޸ĳ� **1** �����ˡ�

> �����smaliָ���Ϥ������Ի�10����ȥ�˽�һ��smali�Ļ����﷨��

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bba10c172083?w=973&h=273&f=png&s=17650"/>

����һ��string���͵ĳ��� **v1**����ֵΪ **1**�����������س�ȥ��

### ��̬����

�ƽ���������̫���ˣ���ʡ���˵��Բ��裬�Ǿ�ֱ��

**���棬�㶨��**

## �ر�

�������ѷ������������ļ��������»ر�� apk��

### ���´��

cmd��apktool�ļ������棬ִ��

```cmd
    apktool b [�ļ�������·��] -o [apk���·��]
```

����޸�smali�ļ�û������Ļ����Ϳ�����������һ���µ� apk �ļ���

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bc841441cecd?w=352&h=112&f=png&s=12086"/>

��ʱ��ֱ�ӽ����´����apk�ļ���ȥ��װ�ǲ��еģ���Ϊ֮ǰzip��ѹ��Ŀ¼�У�**META-INF** �ļ��о��Ǵ��ǩ����Ϣ��Ϊ�˷�ֹ���⴮�ġ�

**����������Ҫ�����´����apk����ǩ����**

### ����ǩ��

����׼��һ�� **.jks** ��ǩ���ļ����������android��ͬѧӦ�ú���Ϥ�ˡ�

������JDK����������ֱ��ִ�У�

```cmd
    jarsigner -verbose -keystore [ǩ���ļ�·��] -storepass [ǩ���ļ�����] -signedjar [��apk���·��] -digestalg SHA1 -sigalg MD5withRSA [��apk����·��] [ǩ���ļ�����]
```

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bd533315f491?w=668&h=199&f=png&s=27954"/>

���������ļ������棬�Ϳ��Կ���һ�� **ĳèVIP�ƽ��.apk**��

��װ����֤����

<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bdf4d548b877?w=540&h=960&f=jpeg&s=21468" width="270" hegiht="480" align=center />
<img src="https://user-gold-cdn.xitu.io/2019/8/10/16c7bdc646e4b4b7?w=720&h=1280&f=jpeg&s=19961" width="270" hegiht="480" align=center />

## �ܽ�

���������һ���ƽ����̣�

**1����ԭӦ�� apk ��׺�ĳ� zip����ѹ�� classes.dex �ļ�**

**2��ʹ�� dex2jar �� classes.dex ת�� jar �ļ�**

**3���� jar �ļ��� jd-gui �򿪣��鿴Դ����**

**4��adb��λ��������·�����ҵ���ش���**

**5��apktool ������ apk���ҵ� smali ��Ӧ�ı��Ƶ�**

**6���޸� smali �ļ������Գ���**

**7�����´��������ǩ��**

�������Ҷ�����ƽ����̵�һ���ܽᣬ����в��Ի�����©�ĵط��������λ����ָ����

����е��ð���ɿ�һ�������˻������������뵽С�ջ���������Ǿ仰��**���ӿ����ϲ��ã�����Ƿ���**����Ҳ�ͷ������ƣ����ڿյ��ķ��䣬����ϲ���ɵ���^_^����Ҳ�ǸսӴ�Android����û��ã�һ��ʼ��Ϊ�ܸ��ӣ����鷳����ʱֻ�Ǳ������������Ե���̬�����������������ˣ�û�뵽ֻ����һ����Сʱ����Ȼ�ͳɹ��ˣ���û�������е���ô�ѡ�

����������Ҳ����Ȥ�Ļ������Һ���һ���ǳ�ѧ�ߣ��Ҿ������ʵս���̷ǳ��ʺ��㡣һ����������ܵ��ƽ���������̣������ѶȲ��󣬲������������Ȥ��ͬʱ���ܵõ�һ���ĳɾ͸С�

## License

    Copyright 2019 goldze(������)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.