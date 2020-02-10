## babel-macro-del-new 删除new关键词

将大写开头的`CallExpression`转化为`NewExpression`

- [@babel/types](https://babeljs.io/docs/en/babel-types)
- [astexplorer](https://astexplorer.net/)


```js
Ajanuw("h")
__Ajanuw("h")
new Ajanuw()
hello()

o.Ajanuw()
o.x.Ajanuw('h')
new o.Ajanuw()

o['Ajanuw']()
o['ajanuw']()
```
to
```js
new Ajanuw("h");
new __Ajanuw("h");
new Ajanuw();
hello();
new o.Ajanuw();
new o.x.Ajanuw('h');
new o.Ajanuw();
new o['Ajanuw']();
o['ajanuw']();
```
