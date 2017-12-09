# Parcel Example - React Counter

<!-- 使用 [Parcel](https://parceljs.org/) 打包的 React Counter 应用。

## 0. 新建目录

    mkdir react-counter
    cd react-counter

## 1. 初始化 npm

    npm init -y

此时会创建要给 package.json 文件，文件内容：

```json
{
  "name": "parcel-example-react-counter",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}
```

## 2. 添加 React

npm:

    npm install react react-dom --save

package.json 文件内容：

```diff
 {
   "name": "parcel-example-react-counter",
   "version": "1.0.0",
   "description": "",
   "main": "index.js",
   "scripts": {
     "test": "echo \"Error: no test specified\" && exit 1"
   },
   "keywords": [],
   "author": "",
-  "license": "ISC"
+  "license": "ISC",
+  "dependencies": {
+    "react": "^16.2.0",
+    "react-dom": "^16.2.0"
+  }
 }
```

## 3. 添加 Babel

新建 .babelrc 文件

    touch .babelrc

输入内容：

```json
{
  "presets": ["react"]
}
```

添加 babel-preset-react：

npm:

    npm install babel-preset-react --D

此时 package.json 文件内容：

```diff
 {
   "name": "parcel-example-react-counter",
   "version": "1.0.0",
   "description": "",
   "main": "index.js",
   "scripts": {
     "test": "echo \"Error: no test specified\" && exit 1"
   },
   "keywords": [],
   "author": "",
   "license": "ISC",
   "dependencies": {
     "react": "^16.2.0",
     "react-dom": "^16.2.0"
-   }
+   },
+   "devDependencies": {
+     "babel-preset-react": "^6.24.1"
+   }
 }
```

## 5. 添加 Parcel


npm:

    npm install parcel-bundler --D

此时 package.json 文件内容：

```diff
 {
   "name": "parcel-example-react-counter",
   "version": "1.0.0",
   "description": "",
   "main": "index.js",
   "scripts": {
     "test": "echo \"Error: no test specified\" && exit 1"
   },
   "keywords": [],
   "author": "",
   "license": "ISC",
   "dependencies": {
     "react": "^16.2.0",
     "react-dom": "^16.2.0"
    },
    "devDependencies": {
-      "babel-preset-react": "^6.24.1"
+      "babel-preset-react": "^6.24.1",
+      "parcel-bundler": "^1.0.3"    
    }
 }
```

## 6. 新建 index.html 文件

内容

```html
<html>

<body>
    <div id="root"></div>
    <script src="./index.js"></script>
</body>

</html>
```

## 7. 新建 js 文件

创建 

- index.js
- app.jsx

## 8. 添加打包命令

```diff
 {
   "name": "parcel-example-react-counter",
   "version": "1.0.0",
   "description": "",
   "main": "index.js",
   "scripts": {
-    "test": "echo \"Error: no test specified\" && exit 1"
+    "start": "parcel index.html"
   },
   "keywords": [],
   "author": "",
   "license": "ISC",
   "dependencies": {
     "react": "^16.2.0",
     "react-dom": "^16.2.0"
    },
    "devDependencies": {
       "babel-preset-react": "^6.24.1"
       "babel-preset-react": "^6.24.1",
       "parcel-bundler": "^1.0.3"    
    }
 }
```

## 9. 完成 -->

    npm start

打開 <http://localhost:1234>

打包完畢會產生 .cache 和 dist 兩個資料夾。

.gitignore

```
.cache
dist
node_modules
```
