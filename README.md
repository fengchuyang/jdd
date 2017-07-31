#jdd
js文档，demo和说明文档快速生成

##快速入门

cmd命令行窗口下执行

	jdd

会生成首页,demo页,changelog页,api页

##目录结构

	demo/ demo文件目录
	js/ js文件目录
	doc/ 说明文件目录
	changelog.md
	readme.md
	package.json

##配置详解

	{
		"name": "myjs",  //工程名
		"version": "1.0.0", //版本号
		"author": "fe", //作者
		"api": {
			"name": "jds api", //js api工程名,会显示api首页
			"description": "" //js api工程描述,同样会显示在api首页
		},
		"apisource":"js/", //js目录
		"demosource":"demo/", //demo目录
		"demoExclude":"demoExcludeDir", //demo目录过滤
		"docsource":"doc/", //说明文档目录
		"target":"docs/", //生成到目录
		"demopathprefix":"../", //demo页导航url前缀
		"stat":"" //统计代码
		"extendHtml":"",//在页面最底部增加额外的html片断
		"copyright":"",//底部版权信息
		"extendMenu":{
			"http://a.com":"这是站点a", //导航上增加额外的链接
			"http://b.com":"这是站点b"
		}
	}

##建议package.json源文件

可直接复制后生成package.json

	{
		"name": "myjs",
		"version": "1.0.0",
		"author": "fe",
		"api": {
			"name": "jds api",
			"description": ""
		},
		"apisource":"js/",
		"demosource":"demo/",
		"docsource":"doc/",
		"target":"docs/",
		"demopathprefix":"../",
		"copyright":"Copyright © 2015 xxx All Rights Reserved"
	}