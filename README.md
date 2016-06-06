# CodeStandards
code satandards for Grouplus fronter 

## 0. 约定规则

1. 变量: 永远不用-来作为分隔符,均采用_分割,除css
2. 复制粘贴,需要谨慎!

## 1. PHP

1. 文件名 & 类名: 均采用大写驼峰开头
2. 变量         : 下划线编码,尽量与后端wiki保持一致
3. 方法         : 小写开头驼峰
4. 顺序         : 命名变量/class/方法时,主要采取`实体-具体操作`,例如给活动修改基本信息的方法应该命名为`basicInfoUpdate`
5. `@include()` : 有相同的html代码,尽量用include进行模块化.但注意,模块间的嵌套尽量控制在3层内,极度情况下最多使用4层
6. Model声明接口: 声明接口字符串与wiki中应该一致,不要使用字符串拼接,而使用字符串替换(商量)
7. Model参数调用: 当接口url中需要的参数,都单独占一个参数,其他的params参数在controller整理好后才统一给Model传
7. route表      : 前端的action请求名必须和Controller方法名称一样
8. json返回     : err_code和后台一致,err_msg替换为中文信息,待定

## 2. html & js

1. 文件名 & 对象 : 
  1. 若js为对象js(例如BasicInfo.js/MoreInfo.js),采用大写驼峰开头
  2. 若为非对象js,采用小写开头驼峰(?现在很多都是以_分割命名js,这里有争议)
2. 控件的id取值  : 
  1. id与wiki中的属性有直接关系时候,id与wiki中的属性一致
  2. 当input的hidden控件中,要保存与wiki中相同的字段时,必须命名为`hid_字段值`
  3. 当觉得id命名需要增加控件类型时,例如`btn` `input` 等,必须加在id的最前面
3. blade.php     : 命名必须为下划线分割(争议?采用小写开头驼峰)
4. 选择器        : 尽可能少的使用一连串.class来作为选择器
5. 控件属性顺序  : type>id>class>value 
