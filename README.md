# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

---

正常正文

**加粗正文**

*倾斜正文*

~~删除正文~~

<u>下划线正文</u>


---

脚注示例，这是一个 Markdown[^1] 文本

> 引用示例
> > 嵌套引用示例

行内代码 `printf()` 示例

```kotlin
/**
 * 代码示例
 * */
class Test {
    private val aa = "hello"
}
```
---

有序列表

1. 测试测试
2. 测试测试
3. 测试测试

无序列表

- 测试测试
- 测试测试
- 测试测出


---

[链接示例](https://www.baidu.com)

<https://www.runoob.com>

---

这是一个图片示例

![图片](https://img.shields.io/badge/Markdown-%E6%B5%8B%E8%AF%95%E5%9B%BE%E7%89%87-green)

---

表格（默认左对齐）

| 一 | 二 | 三 | 左对齐 | 右对齐 | 居中对齐 |
| - | - | - | :- | -: | :-: |
| 1 | 2 | 3 | A | A | A |
| 4 | 5 | 6 | B | B | B |
| 7 | 8 | 9 | C | C | C |

---
支持 Html 元素

`<kbd>`：<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd>

`<b>`：<b>文本加粗</b>

`<i>`：<i>文本倾斜</i>

`<em>`：<em>文本倾斜</em>

`<sup>`：一段演示文本<sup>脚注</sup>

`<sub>`：一段演示文本<sub>脚注</sub>

转义字符 

正常显示星号 \*

公式

行内公式

$f(x) = sin(x) + 12$

块内公式

$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$

---
Github 中支持了 `mermaid` 绘图工具，用于绘制流程图、甘特图等

> 注意：此特性不是所有的 markdown 解释器都会支持！

```mermaid
---
title: 横向流程图
---
graph LR
A[方形] -->B(圆角)
    B --> C{条件a}
    C -->|a=1| D[结果1]
    C -->|a=2| E[结果2]
```

```mermaid
---
title: 竖向流程图
---
graph TD
A[方形] --> B(圆角)
    B --> C{条件a}
    C --> |a=1| D[结果1]
    C --> |a=2| E[结果2]
```

```mermaid
sequenceDiagram
    title 时序图例子
    participant 张三
    participant 李四
    张三->王五: 王五你好吗？
    loop 健康检查
        王五->王五: 与疾病战斗
    end
    Note right of 王五: 合理 食物 <br/>看医生...
    李四-->>张三: 很好!
    王五->李四: 你怎么样?
    李四-->王五: 很好!
```

```mermaid
---
甘特图例子
---
gantt
    title 甘特图例子 from 官方
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```
```mermaid
---
title: Git 流程图
---
gitGraph
    commit
    commit
    branch develop
    checkout develop
    commit
    commit
    checkout main
    merge develop
    commit
    commit
```

[^1]: Markdown是一种纯文本标记语言
