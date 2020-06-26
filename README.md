# WeiXinCalendar
微信小程序-日历组件

通过设置时间、假期来展示一个可显示规定日期的放假、休息状态

## 使用
- `git clone https://github.com/380428652/WXCalendar` 到本地
- 把 `page` 中的 `date` 拷贝到自己项目下。
- 在使用页面注册组件
  ```json
  {
    "usingComponents": {
      "component-date": "/page/date/date"
    }
  }
  ```
- 在页面 `**.wxml` 文件中加入如下代码
  ```html
  <component-date year="2018" start_month="9" end_month="12" rest="9-1,9-27,9-8,10-9" vacation="9-3,9-18,10-4,11-8,12-3" bind:click="onClick" isClick="false" current="9-11"></component-date>
  ```
## Api
自定义年份（year）、起止月份（start_month、end_month）、休息日（rest）、假日（vacation）、当天时间（current）、点击返回日期（click）、点击事件是否禁用（isClick）
