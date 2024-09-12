# WJStudy
前后端分离项目设计

20240912记录：
解决前端登录跳转问题

修改位置：
wj-vue\src\main.js

原：

var axios = require('axios')

axios.defaults.baseURL = 'http://localhost:8443/api'

改：

import axios from 'axios'

Vue.prototype.$axios = axios

axios.defaults.baseURL = 'http://localhost:8443/api'
