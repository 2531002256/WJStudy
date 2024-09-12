# WJStudy
前后端分离项目设计

## 20240912记录：
### 解决前端登录跳转问题

#### 修改 wj-vue\src\main.js

原：

var axios = require('axios')

axios.defaults.baseURL = 'http://localhost:8443/api'

改：

import axios from 'axios'

Vue.prototype.$axios = axios

axios.defaults.baseURL = 'http://localhost:8443/api'

### 解决数据库连接问题
#### 修改pom.xml文件
mysql依赖修改：5.1.21 ---》 5.1.46

