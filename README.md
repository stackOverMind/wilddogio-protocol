# wilddogio-protocol
这个模块为wilddog 云端与js客户端共用模块
此模块定义了同步操作中的所有子操作,并对其序列化与反序列化
具体操作有:
* 添加数据
* 推送数据
* 删除数据
* 修改数据
* 订阅数据
* 查询数据

## API


### ref=WDProtocal(baseUrl)
初始化客户端

### ref.add(data,callback)
添加数据
###### arguments
* data
{path:&lt; path &gt;,data:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}
* callback
function(err):如果err null 操作成功

###### return
* null

### ref.push(data,callback)
推送数据

###### arguments
* data:{path:&lt;path&gt;,data:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}
* callback
function(err):如果err null 操作成功

###### return
* null

### ref.delete(data,callback)
删除数据

###### arguments
* data:{path:&lt;path&gt;,[opt:{&lt;optional data&gt;}]}
* callback
function(err):如果err null 操作成功

###### return
* null

### ref.update(data,callback)
修改数据

###### arguments
* data:{path:&lt;path&gt;,data:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}
* callback
function(err):如果err null 操作成功

###### return
* null

### ref.subscribe(data,callback)
订阅数据

###### arguments
* data
{path:&lt;path&gt;,[opt:{&lt;optional data&gt;}]}
* callback
function(err,data):如果err null 操作成功,如果操作成功data是一个object {path:&lt;path&gt;:data:{&lt;data&gt;}}

###### return
* null

### ref.query(data,callback)
查询数据

###### arguments
* data
{path:&lt;path&gt;,query:&lt;query&gt;,[opt:{&lt;optional data&gt;}]}
* callback

function(err,data):如果err null 操作成功,如果操作成功data是一个object {path:&lt;path&gt;,data:{&lt;data&gt;}[opt:{&lt;optional data&gt;}]}

###### return
* null

### ref.onAdd(callback)
监听添加数据事件

###### arguments
* callback
function(err,data):如果err null 操作成功,如果操作成功data是一个object {path:&lt;path&gt;,data:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}

###### return
* null

### ref.onPush(callback)

###### arguments
* callback
function(err,data):如果err null 操作成功,如果操作成功data是一个object {path:&lt;path&gt;,data:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}

#### return
*null

### ref.onDelete(callback)

###### arguments

###### return
*null



