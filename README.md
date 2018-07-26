# hutianhao.github.com
### 关于图像风格迁移服务器接口的说明
- url：	http://ai.jinmensuyin.com:15004/upload
- 方法：	http  post
- 内容：表单	'style=face'   
		style=xxx，表示图片文件需要转化成的风格类型，其中xxx为下面的值之一   
		"star" 梵高星空风格   
		"face" 人脸素描风格   
		"gold" 抽象金色风格   
		"chouxiang"毕加索风格   
		"girl"哥特玻璃风格   
		"scream"蒙克尖叫风格   
		
2. 文件：需要转化风格的原文件
		
- 测试访问：   
浏览器：http://ai.jinmensuyin.com:15004/upload   
linux curl：	curl -X POST 'http://ai.jinmensuyin.com:15004/upload'  -F 'style=face' -F "file=@1.jpg"	
其中，	-F "file=@1.jpg"	表示上传当前目录的文件1.jpg，
			-F 'style=face'		表示上传表单'style=face'	

- 测试条件：	手机和电脑IP须在北邮校园网内部。因为，服务器目前在实验室。

- 微信h5界面设计说明：   
1. 参考界面 http://ai.jinmensuyi1.com:15004/upload
2. 设计一个手机的上传页面，供用户选择风格类型和文件
3. 用户点击上传后，按照上述接口，post表单和文件到服务器
4. 最终手机上，显示风格迁移后的目标图片


