## Local Library

## what i gonna do?
* use express application generator to build an application skeleton.
* boot and stop the Node web server.
* use database to store the application data.
* create routers to handle different requests, create model(view) to render HTML data to display on the browser.
* use forms.
* deploy the application on the prodction environment.

## 数据库选择
MongoDB、ODM框架Mongoose

数据模型：
书信息（书名、摘要、作者、种类、ISBN）

## 后端路由

catalog/：主页。
catalog/<objects>/：模型（藏书、藏书副本、藏书种类、作者）的完整列表（例如 /catalog/books/、/catalog/genres/ 等）
catalog/<object>/<id>：具有 _id 字段值的特定模型的详细信息页面（例如 /catalog/book/584493c1f4887f06c0e67d37）。
catalog/<object>/create：添加新模型的表单（例如 /catalog/book/create）。
catalog/<object>/<id>/update：更新具有 _id 字段值的特定模型的表单（例如 /catalog/book/584493c1f4887f06c0e67d37/update）。
catalog/<object>/<id>/delete：删除具有 _id 字段值的特定模型的表单（例如 /catalog/book/584493c1f4887f06c0e67d37/delete）。

## 遇到的问题

* throw new MongooseError('Model.prototype.save() no longer accepts a callback');
https://www.saoniuhuo.com/question/detail-2513383.html