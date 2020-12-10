# Cookie 参数

你可以采用与定义 `Query` 和 `Path` 参数相同的方式来定义 Cookie 参数。

## 导入 `Cookie`

首先要导入 `Cookie`:

```Python hl_lines="3"
{!../../../docs_src/cookie_params/tutorial001.py!}
```

## 申明 `Cookie` 参数

然后以与申明 `Path` 和 `Query` 相同的语法结构申明 cookie 参数。

第一个是默认值，你可以传入额外的校验和注释参数：

```Python hl_lines="9"
{!../../../docs_src/cookie_params/tutorial001.py!}
```

!!! 技术细节
    `Cookie` 是 `Path` 和 `Query` 的 "姊妹" 类。它也继承自同一个 `Param` 类。

    但请记住当你从 `fastapi` 中导入 `Query`, `Path`, `Cookie` 等等时，它们实际是返回特定类的函数。

!!! Info
    必须使用 `Cookie` 来申明 cookies， 否则参数会被解释成 query 参数.

## 回顾

使用与 `Query` and `Path` 相同的语法格式来申明 `Cookie` 。
