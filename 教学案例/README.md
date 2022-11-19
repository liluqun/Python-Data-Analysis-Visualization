![Python与数据分析及可视化](https://imgservice.suning.cn/uimg1/b2c/image/gIH3lXgAHfqhSFy_QvLmpQ.jpg_800w_800h_4e)
# Prof.Li's Python Education Tools

## Author: 道法自然

## **模块安装：pip install -U python-education-tools**

* Python Education Tools模块为教材配套工具。模块由作者Prof.Luqun Li团队自主开发 。
* 模块简称“pet工具”。取Python Education Tools 首字母的缩写pet（英文意思：宠物），希望该工具成为大家学习的宠物！。
* 所有工具包的根目录是pet。模块安装后对应的安装包为 pet.data.* 、pet.textbook1.*等。
* 今后会根据大家的需求，不断扩充相关教学相关工具和数据集。如果您有好的建议，请发邮件到liluqun@gmail.com联系我。

![hah](https://tse1-mm.cn.bing.net/th/id/OIP-C.1WzofyXU4XlVG1soFYMmpgHaEc?w=273&h=180&c=7&r=0&o=5&dpr=2&pid=1.7)

`````

** Pet相关模块的使用：**

1.教材配套的案例下载（运行以下1行Python代码）：
 
      import pet.textbook1.codes
      稍后，即可将教学案例下载到桌面教学案例目录。
  
2.趣谈编程之道（运行以下1行Python代码）：
  
      import pet.this
      与“晦涩难懂的”Python编程之禅import this对应，本模块从中国传统文化，心，术，道三个层次，引用古文阐述编程之道。
      内容大家自己体会，道法自然，道不简则理不明！！Just for Fun！！！（不笑不足以为道!!)

3.教材相关的样本数据加载：

   from pet.data import load_data
   df1 = load_data.load_data(数据集名称)
            '''
            数据集名称如下：
                'ip_address.xlsx'  -ip地址分类。返回：dataframe
                'st.xls' -某高校研究生初试成绩。返回：dataframe
                'subway.xlsx'  -上海地铁线路数据。返回：dataframe
                'ddj.txt' -道德经文本。返回：字符串。
                'tyjhzz.txt'-《太乙金华宗旨》。返回：字符串。
                '2022pst.xlsx'-2022年优秀毕业论文。返回：dataframe。
                '2022tsk.xlsx'-2022年通识课。返回：dataframe。
                'beijing_bus.xlsx'-北京公交车信息。返回：dataframe。
            今后将陆续增加数据集。
            '''
            其它数据：
                load_data.votes #投票文本数据
                load_data.cookies  #某cookies数据

4.伪数据集的随机生成函数：

    以下2个函数可以分别随机生成Series和DataFrame对象数据。
    
    dffs = load_data.generate_sr(rows=100)
        '''
        生成一个Series对象，对象内数据条数默认40条，可任意设置。
        '''
    dfff = load_data.generate_df(rows=200)
        '''
        生成一个Dataframe对象，对象内数据条数默认40条，可任意设置。shape是（n，13），n为数据条数
        '''


`````

![hah](https://img.niuqiuyi.com/202210/19/012355471.png)