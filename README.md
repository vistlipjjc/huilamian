#前端项目开发说明

## 一、开发环境运行说明

### 1 安装npm淘宝镜像
如果有则忽略此步骤

`npm install -g cnpm --registry=https://registry.npm.taobao.org`

### 2 安装依赖模块
`cnpm install`

### 3 启动项目
`npm run dev`

## 二、开发命名规范

### views 下的文件夹命名
1. views 下面的文件夹代表着模块的名字
2. 驼峰命名，小写开头
3. 由名词组成（home、 message）

### views 下的 vue 文件命名
1. views 下面的 vue 文件代表着页面的名字
2. 驼峰命名，小写开头
3. 由名称组成
4. 开头单词就是所属模块名字（如：staffList、staffEdit、staffView）

### method 自定义方法命名
1. 驼峰命名，小写开头
2. 由动宾短语组成
2. 查询列表数据，分页：query、 不分页：select
3. 获取单条数据，get
4. 尽量使用常用单词开头（如：query、select、get、add、remove、refresh、……）

### 生命周期方法注意点
1. 不在 created, mounted 之类的方法内写逻辑、取 Ajax 数据。

### vue 文件内引用组件
1. html 内引用自定义组件以小写加短线（如：`<j-table></j-table>`）