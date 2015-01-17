# wilddogio-protocol


## 连接操作
* eventType:conn

### handshake
{"seq":&lt;seq&gt;,"app-id":"&lt;app id&gt;" }

### disconnect


## 数据操作
* eventType:data
### on

{"action":"&lt;query&gt;","seq":&lt;seq&gt;,"path":"&lt;path&gt;"}

### once

{"action":"&lt;query&gt;","once":1,"seq":&lt;seq&gt;,"path":"&lt;path&gt;"}

### push

{"action":"&lt;push&gt;","seq":&lt;seq&gt;,"path":"&lt;path&gt;","data":&lt;data&gt;}

### update

{"action":"&lt;modify&gt;","seq":&lt;seq&gt;,"path":"&lt;path&gt;","data":&lt;data&gt;}

### set

{"action":"&lt;push&gt;","seq":&lt;seq&gt;,"path":"&lt;path&gt;","data":&lt;data&gt;}

### delete

{"action":"&lt;push&gt;","seq":&lt;seq&gt;,"path":"&lt;path&gt;","data":null}
