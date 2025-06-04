[[supabase教程]]

## 流程
1. 下载next.js的官方supabase模版
	1. 下载链接：https://vercel.com/templates/authentication/supabase
	2. 下载命令
		1. ```pnpm create next-app --example with-supabase with-supabase-app```
	3. 编写next.js代码
		1. 提示词：请你帮我生成-个超级好看的todo list页面，要求酷炫一点，采用tailwindcss + lucide-react的icon!
	4. 修改相关页面
		1. 提示词：1、@auth 登陆注册相关页面的配色和 @page.tsx 首页保持一致  
                 2、 @page.tsx 增加登陆和注册按钮，跳转对应的页面
2. 配置supabase数据库
	1. `填写key 和url`
	2. 填写提示词:  
```
@page.tsx 请你结合 @init.sql 数据表；使用supabase链接到真实的数据库中，要求实现：  
1.当前页面用户登录后，用登录态时请求用户的todo数据  
2.实现用户增加任务，并保存的功能  
3.实现用户删除todo，并保存的功能3.实现用户修改操作，并保存的功能  
4.实现用户点击完成，修改完成状态并保存的功能5.确保查询、修改、删除的是当前用户的数据
```
3. 增加图片功能
	1. 创建bugket桶
	2. 数据库增加image_ul字段
	3. 提示词：
```我希望给Todo项增加图片上传功能:  
1.运行用户上传图片到当前增加的todo中，作为附件，只允许上传一个附件  
2.附件需要先上传到名字为my-todo的bucket中(已有该bucket)，路径为该用户uid的目录下，并返回附件的预览地址  
3.附件的预览地址，需要保存在数据库中，请你结合sql @init.sql 字段为image_url!
```
4. 增加realtime功能
	1. 提示词：
`@page.tsx 请你给这个应用增加supabase realtime功能:
1.用户更新自己的数据后，todos这张表的数据能够同步的在其他设备的浏览器中更新
2.确保用户的增加、删除、修改操作都能够触发视图数据的更新`