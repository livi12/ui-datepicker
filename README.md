#ui-datepicker插件的使用

乐课网使用的时间选取插件是调用的[My97日期插件](http://www.my97.net/dp/license.asp),具体的[参数配置](http://www.my97.net/dp/demo/index.htm)的配置说明。根据需求复写配置属性

##乐课中ui-datepicker插件的使用

###html
添加Wdate会给输入框添加日历图标，如下图
![日历图标](http://192.168.20.21:8080/gitbucket/Tracy/widget/blob/master/widget/ui-datepicker/images/Wdate.png "日历图标")

```html
<input type="text" id="jStartDate" name="stDate" class="u-ipt u-ipt-nm Wdate" readonly="">
```

###javascript调用
给指定的元素绑定点击事件，生成日历，并进行配置一些参数，具体参数查看[参数配置](http://www.my97.net/dp/demo/index.htm)

```javascript
$('#jStartDate').click(function(){
	WdatePicker({
		dateFmt:'yyyy-MM-dd',
		readOnly:true
	});
});
```