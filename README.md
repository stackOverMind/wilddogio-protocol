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
* data:{t:"a",p:&lt; path &gt;,d:{&lt;data&gt;},[opt:{&lt;optional data&gt;}]}
* callback

###### return
* null

### ref.push(data,callback)
推送数据

###### arguments
* data:{t:"p",p:<path>,d:{<data>},[opt:{<optional data>}]}
* callback

#### return
* null

### ref.delete(data,callback)
删除数据

###### arguments
* data:{t:"d",p:<path>,[opt:{<optional data>}]}
* callback

###### return
* null

### ref.update(data,callback)
修改数据

###### arguments
* data:{t:"u",p:<path>,d:{<data>},[opt:{<optional data>}]}
* callback

#### return
* null

### ref.subscribe(data,callback)
订阅数据

#### arguments
* data:{t:"s",p:<path>,[opt:{<optional data>}]}
* callback

#### return
* null

### ref.query(data,callback)
查询数据

#### arguments
* data{t:"q",p:<path>,q:<query>,[opt:{<optional data>}]}
* callback

#### return
* null

### ref.onAdd(callback)
监听添加数据事件

#### arguments
* callback:function(path,data,[optional])

#### return
* null

### ref.onPush(callback)
#### arguments

#### return




