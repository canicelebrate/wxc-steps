# wxc-steps

> 步骤条 - 小程序组件

## Install

``` bash
$ min install @canicelebrate/wxc-steps
```


## API

### 代码演示
在模板中使用 wxc-steps 模板，并传入相应数据
```html
<wxc-steps type="horizon" steps="{{steps}}"></wxc-steps>
```
| 参数       | 说明      | 类型       | 默认值       | 必须      |
|-----------|-----------|-----------|-------------|-------------|
| type | steps 的展示状态，可选值为 'horizon', 'vertical' | String | horizon | |
| hasDesc | 是否展示描述 | Boolean  | false | |
| steps | 步骤条展示数据 | Array  |  | 必须 |
| className | 自定义类目，方便自定义显示 | String  | | |


steps 数据格式如下：
```js
[
  {
    // 此步骤是否当前完成状态
    current: false,
    // 此步骤是否已经完成
    done: true,
    // 此步骤显示文案
    text: '步骤一',
    // 此步骤描述语
    desc: '10.01'
  },
  {
    done: true,
    current: false,
    text: '步骤二',
    desc: '10.02'
  },
  {
    done: true,
    current: true,
    text: '步骤三',
    desc: '10.03'
  }
]
```

## ChangeLog

#### v1.0.1（2018-6-1）
- 初始版本
#### v1.0.2（2018-6-2）
- 完善demo页
