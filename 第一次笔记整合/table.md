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
![alt text](./HTML/img/table_2.png)

### HTML表单

### 1. 表单元素类型

   | type属性值 | 说明       |
   |------------|------------|
   | text       | 文本框，输入单行文本 |
   | password   | 密码框     |
   | radio      | 单选框     |
   | checkbox   | 多选框     |
   | file       | 上传文件   |

### 2. 表单元素示例

   ```html
   <!-- 文本框 -->
   <input type="text" placeholder="输入用户名">

   <!-- 密码框 -->
   <input type="password" placeholder="输入密码">

   <!-- 单选框 -->
   <input type="radio" name="gender">男性
   <input type="radio" name="gender">女性

   <!-- 多选框 -->
   <input type="checkbox">选项1
   <input type="checkbox">选项2

   <!-- 上传文件 -->
   <input type="file">
   ```

### 3. 单选框和多选框的特殊属性

   - **单选框**：
     - 使用 `name` 属性将多个单选框分组，同一组内只能选一个。
     - 使用 `checked` 属性设置默认选中的选项。

   ```html
   <input type="radio" name="gender" checked>男性
   <input type="radio" name="gender">女性
   ```

   - **多选框**：
     - 多选框不需要 `name` 属性分组，每个多选框独立选择。

### 4. 图标和图片的使用

   ```html
   <input type="radio" name="gender" checked>Transgender Girl <img src="./img/Transgender_Pride_flag.svg.png" width="25">
   ```

   - 可以在表单元素旁边添加图片或图标，增强用户体验。


## HTML单选框

### 1. 单选框的基本用法

   ```html
   <input type="radio" name="gender">选项1
   <input type="radio" name="gender">选项2
   ```

   - `type="radio"` 定义单选框。
   - `name` 属性用于将多个单选框分组，同一组内只能选一个选项。

### 2. 设置默认选中项

   ```html
   <input type="radio" name="gender" checked>选项1
   <input type="radio" name="gender">选项2
   ```

   - 使用 `checked` 属性设置默认选中的选项。

### 3. 单选框与图片结合

   ```html
   <input type="radio" name="gender" checked>Transgender Girl <img src="./img/Transgender_Pride_flag.svg.png" width="25">
   ```

   - 可以在单选框旁边添加图片或图标，增强用户体验。


## HTML文件上传

### 1. 文件上传的基本用法

   ```html
   <input type="file">
   ```

   - `type="file"` 定义一个文件上传控件，允许用户从本地计算机选择文件上传。

### 2. 上传多个文件

   ```html
   <input type="file" multiple>
   ```

   - 使用 `multiple` 属性允许用户选择并上传多个文件。

## HTML多选框默认选中

### 1. 多选框的基本用法

   ```html
   <input type="checkbox">选项1
   <input type="checkbox">选项2
   ```

   - `type="checkbox"` 定义一个多选框，允许用户选择多个选项。

### 2. 设置默认选中项

   ```html
   <input type="checkbox" checked>选项1
   <input type="checkbox">选项2
   ```

   - 使用 `checked` 属性设置多选框的默认选中状态。

   ## HTML下拉选择框

### 1. 下拉选择框的基本用法

   ```html
   <select>
       <option>选项1</option>
       <option>选项2</option>
   </select>
   ```

   - `select` 标签定义一个下拉选择框。
   - `option` 标签定义下拉选择框中的选项。

### 2. 设置默认选中项

   ```html
   <option selected>选项</option>
   ```

   - 使用 `selected` 属性设置下拉选择框的默认选中选项。

   ## HTML文本域

### 1. 文本域的基本用法

   ```html
   <textarea placeholder="请输入评论"></textarea>
   ```

   - `textarea` 标签定义一个多行文本输入控件，允许用户输入较长的文本。
   - `placeholder` 属性提供提示信息，指导用户输入内容。


   ## HTML单选按钮

### 1. 单选按钮的基本用法

   ```html
   <input type="radio" name="gender" id="man"> <label for="man">男</label>
   <input type="radio" name="gender" id="woman"><label for="woman">女</label>
   ```

   - `type="radio"` 定义一个单选按钮，允许用户在一组选项中选择一个。
   - `name` 属性用于将一组单选按钮分组，同一组内的单选按钮只能选择一个。
   - `id` 属性为单选按钮定义一个唯一标识符。
   - `label` 标签与 `for` 属性结合使用，为单选按钮添加描述性文本，并提高可访问性。

### 2. 简化标签的使用

   ```html
   <label><input type="radio" name="gender">女</label>
   ```

   - 将 `input` 标签嵌套在 `label` 标签内，简化了HTML结构，同时保持了与单选按钮的关联。

   ## 列表
   
   1. 无序列表
   
      ```html
      <ul>
          <li>1</li>
          <li>2</li>
          <li>3</li>
      </ul>
      ```
   
      > ul只能放li
   
   2. 有序列表
   
      ```html
      <ol>
          <li>1</li>
          <li>2</li>
          <li>3</li>
      </ol>
      ```
   
      > 自动添加数字序号，ol只能包li
   
   3. 定义列表
   
      ```html
      <dl>
          <dt>服务中心</dt>
          <dd>申请售后</dd>
          <dd>售后政策</dd>
      </dl>
      ```
   
      > dl只能包含dt和dd，dt和dd可以包含任何内容
      >
      > dl嵌套dt和dd，dl是定义列表
      >
      > dt是定义列表的标题，dd是定义列表的描述/详情。
   
   ## 案例
   
   ![](./HTML/img/列表案例.png)
   