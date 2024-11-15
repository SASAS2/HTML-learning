## 表格

### 表格基础语法

#### 语法
表格为table标签，行为tr(tablerow)标签，每行可包含多个由td(tabledata)标签定义的单元格,单元格可包含文本，图片，视频，表格，列表等元素。

表格头可使用thead标签定义，表格尾可使用tfoot标签定义。
#### 示例
```html
<table border="1"> 
    <thead>
        <tr>
            <th>C1</th>
            <th>C2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>C1R1</td>
            <td>C1R2</td>
        </tr>
        <tr>
            <td>C2R1</td>
            <td>C2R2</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td>C1F</td>
            <td>C2F</td>
        </tr>
    </tfoot>
</table>
```    

  > border:边框厚度

#### 效果
![alt text](./HTML/img/table_1.png)

## 表格合并

#### 语法
rowspan属性设定单元高度(最上优先) \
colspan属性设定单元宽度(最左优先)

#### 示例
```html
<table border="1"> 
    <thead>
        <tr>
            <th>C1</th>
            <th>C2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2">C1R1</td>
            <td>C1R2</td>
        </tr>
        <tr>
            <td>C2R2</td>
        </tr>
    </tbody>
</table>
```
#### 效果
![alt text](/HTML/img/table_2.png)