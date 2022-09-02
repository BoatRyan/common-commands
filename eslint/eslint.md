## eslint

### eslint配置文件

eslint 中所有的检测规则都是可配置的，自然所有的配置规则都需要有一个配置的存储文件。

eslint配置文件写在项目根目录下的.eslintrc.*中，文件格式支持js、json、yaml。

### 使用eslint配置文件的优先级

从项目中向上查找，各个项目需要的共同配置放到根级别的eslint配置文件中，`root: true`可以停止查找，让项目只使用自己的配置

### .eslint.json（根据eslint --init 选择对应选项默认生成）

    {
        "env": {
            "commonjs": true,
            "es2021": true
        },
        "extends": "standard",
        "overrides": [
        ],
        "parserOptions": {
            "ecmaVersion": "latest"
        },
        "rules": {
        }
    }

### 配置字段查询

https://cn.eslint.org/docs/user-guide/configuring

### 规则

https://cn.eslint.org/docs/rules/