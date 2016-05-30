# CodeStandards
code satandards for Grouplus fronter 

## 0. 约定规则

1. 变量: 永远不用-来作为分隔符,均采用_分割,除css
2. 复制粘贴,需要谨慎!

## 1. PHP

1. 文件名 & 类名: 均采用大写驼峰开头
2. 变量       : 下划线编码,尽量与后端wiki保持一致
3. 方法       : 小写开头驼峰
4. 顺序       : 命名变量/class/方法时,主要采取`实体-具体操作`,例如给活动修改基本信息的方法应该命名为`basicInfoUpdate`

## 2. html & js

1. 文件名 & 对象 : 
  1. 若js为对象js(例如BasicInfo.js/MoreInfo.js),采用大写驼峰开头
  2. 若为非对象js,采用小写开头驼峰(?现在很多都是以_分割命名js,这里有争议)
2. 控件的id取值  : 
  1. id与wiki中的属性有直接关系时候,id与wiki中的属性一致
  2. 当input的hidden控件中,要保存与wiki中相同的字段时,必须命名为`hid_字段值`
  3. 当觉得id命名需要增加控件类型时,例如`btn` `input` 等,必须加在id最前面
3. blade.php: 命名必须为下划线分割
4. 拒绝用样式来作为选择器绑定任何事件.
