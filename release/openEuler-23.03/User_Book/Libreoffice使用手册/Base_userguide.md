# LibreOffice Base使用说明

在 LibreOffice Base 中，您可以访问以各种数据库文件格式存储的数据。LibreOffice Base 本身支持某些平面文件数据库格式，例如，dBASE 格式。也可以使用 LibreOffice Base 连接到外部关系数据库，例如，MySQL 或 Oracle 数据库。

## 1.使用说明

### 1.1 创建与打开数据库

#### 1.1.1 新建数据库

1、选择「文件 - 新建 - 数据库」。这将打开数据库向导，您可以在其中创建一个新的数据库文件。

2、在「数据库向导」中，选择数据库类型，然后选择此选项打开作为下一向导的「表格向导」。表向导可帮助您将表添加到新的数据库文件中。


#### 1.1.2 导入数据库

- 可以从CSV、Spreadsheet（表格）等地方导入数据库

![导入数据库.png](./Pictures/%E5%AF%BC%E5%85%A5%E6%95%B0%E6%8D%AE%E5%BA%93.png)

- 选择要导入的文件

![选择导入文件.png](./Pictures/%E9%80%89%E6%8B%A9%E5%AF%BC%E5%85%A5%E6%96%87%E4%BB%B6.png)

- 最后设置

![导入最后设置.png](./Pictures/%E5%AF%BC%E5%85%A5%E6%9C%80%E5%90%8E%E8%AE%BE%E7%BD%AE.png)

#### 1.1.3 打开已创建数据库

要打开数据库文件，请选择文件 - 打开。在文件类型列表框中，选择只查看“数据库文档”。选择数据库文档，并单击打开。

#### 1.1.4 以表格形式打开数据库表

- 点击Tables，在Tables选择一个表打开

![表格形式打开数据库表.png](./Pictures/%E8%A1%A8%E6%A0%BC%E5%BD%A2%E5%BC%8F%E6%89%93%E5%BC%80%E6%95%B0%E6%8D%AE%E5%BA%93%E8%A1%A8.png)

### 1.2 数据源视图

选择「查看 - 数据源」或按「Ctrl + Shift + F4」键可从文本文档或电子表格调用数据源视图。

在左侧，您可以看到数据源资源管理器。如果在其中选择了表格或查询，则会在右侧看到其内容。位于顶部的是表格数据栏。

### 1.3 使用表格

数据存储在表中。例如，您用于电子邮件地址的系统通讯簿是通讯簿数据库的一个表。每个地址都是一个数据记录，在该表中显示为一行。数据记录由数据字段组成，例如名字和姓氏字段以及电子邮件字段。

#### 1.3.1 使用表格向导创建新表格

在 LibreOffice 中，您可以使用表格向导创建一个新表格：

1、打开要创建新表格的数据库文件。

2、在数据库窗口的左窗格中，点击「表格」图标。

3、点击「使用向导创建表格」。

#### 1.3.2 使用设计视图创建新表格

1、打开要创建新表格的数据库文件。

2、在数据库窗口的左窗格中，点击「表格」图标。

3、点击「在设计视图中创建表格」。

然后就可以看到表格设计窗口了。

#### 1.3.3 创建新表格视图

某些数据库类型支持表格视图。表格视图是随数据库一同存储的查询。对于大多数数据库操作，视图的使用方式与表格相同。

1、打开要在其中创建新表格视图的数据库文件。

2、在数据库窗口的左窗格中，点击「表格」图标。

3、点击「创建表格视图」。

您会看到 View Design 窗口，它与Query Design 窗口几乎相同。

### 1.4 使用查询

如果经常要只访问可根据过滤条件定义的数据子集，您可以定义查询。这在本质上是过滤数据新视图的名称。您可以打开查询并以您定义的表格版式查看当前数据。

#### 1.4.1 使用查询向导创建新查询

在 LibreOffice 中，可使用查询向导创建新查询:

1、打开要创建新查询的数据库文件。

2、在数据库窗口的左窗格中，点击「查询」图标。

3、点击「使用向导创建查询」。

#### 1.4.2 使用设计视图创建新查询

1、打开要创建新查询的数据库文件。

2、在数据库窗口的左窗格中，点击「查询」图标。

3、点击「在设计视图中创建查询」。

您会看到查询设计窗口。

### 1.5 使用表单

使用表单，可以定义如何显示数据。打开一个文本文档或电子表格，并插入控件，例如，按钮和列表框。在控件的属性对话框中，可定义表单应该显示的数据。

#### 1.5.1 使用表单向导创建新表单

在 LibreOffice 中，可使用表单向导创建新表单:

1、打开要创建新表单的数据库文件。

2、在数据库窗口的左窗格中，点击「表单」图标。

3、点击「使用向导创建表单」。

#### 1.5.2 手动创建新表单

1、打开要创建新表单的数据库文件。

2、在数据库窗口的左窗格中，点击「表单」图标。

3、点击「在设计视图中创建表单」。

一个新的文本文档打开。使用表单功能插入表单控件。

- 注意：点击「表单」图标，访问在当前数据库窗口中创建的所有表单。此外，可使用「表单功能」图标将数据库表单功能添加到任何 Writer 或 Calc 文档，但这些文档将不会在数据库窗口中列出。

### 1.6 创建报表

报表是一个以有组织的顺序和格式显示您的数据的 Writer 文本文档。在 LibreOffice Base 中，您可以选择在「报表构建器」窗口中使用拖拽来手动创建报表，或者按照「报表向导」中的一系列对话框半自动创建报表。

以下列表为您提供一些决定用哪种方法处理数据的信息：

| 报表构建器          | 报表向导          |
|--------------------|------------------|
| 通过「在设计视图中创建报表」命令启动。 | 通过「使用向导创建报表」命令启动。 |
| 灵活使用报表页眉与页脚；页眉与页脚；多列报表。 | 使用 Writer 模板生成报表文档。 |
| 使用拖拽来定位记录字段或者其他诸如图形或者线条等设计元素。 | 从几个给出的选项中选择排列数据记录的方式。 |
| 生成数据的一次性快照。要查看更新的报表，请再次执行同一个报表来创建带更新数据的 Writer 模板。 | 您可以选择用固定数据生成一次性快照，或者生成「实时」报表，该报表带有当您打开 Base 文件时当前数据的链接。 |
| 将报表保存为 Writer 文本文档。保存关于如何在 Base 文件中创建报表的信息。 | 保存报表和有关如何在 Base 文件中创建报表的信息。 |
| 在右键菜单中选择「打开」或者双击报表名称用当前数据来创建一个新报表。 | 在右键菜单中选择「打开」，或者双击报表名称可看到首次创建时的数据静态快照，或者可创建一个带当前数据的新报表。这要由您在向导中最后一页所做的选择决定。 |
| 在报表名称的右键菜单中选择「编辑」以打开装入了报表信息的「报表构建器」窗口。 | 在报表名称的右键菜单中选择「编辑」来编辑用来创建报表的 Writer 模板文件。 |

#### 1.6.1 在「设计视图」中手动创建新报表

1、打开您想从中创建新报表的数据库文件。

2、在数据库窗口的左侧面板中，点击「报表」图标。

3、点击「在设计视图中创建报表」。

4、遵循报表构建器指南中的说明。

#### 1.6.2 使用报表向导创建新报表

1、打开您想从中创建新报表的数据库文件。

2、在数据库窗口的左侧面板中，点击「报表」图标。

3、点击「使用向导创建报表」。

4、遵循报表向导中的步骤创建报表。

### 1.7 注册和删除数据库

任何数据库文件中的数据都可以注册到已安装的 LibreOffice 实例中。注册意味着告诉 LibreOffice 数据的位置、组织方式、获取数据的方式等等。注册数据库后，您可以使用菜单命令查看 - 数据源来访问文本文档和电子表格中的数据记录。

#### 1.7.1 要注册现有的数据库文件

1、选择 工具 - 选项 - LibreOffice Base - 数据库。

2、点击「新建」并选择数据库文件。

#### 1.7.2 从 LibreOffice 删除注册数据库

1、选择 工具 - 选项 - LibreOffice Base - 数据库。

2、选择数据库文件，然后点击「删除」。

### 1.8 导入与导出 Base 中的数据

导入与导出数据库表格的一种简便方法是将 Calc 用作「帮助应用程序」。

#### 1.8.1 从 Base 中导出数据

将 Base 中的表格复制到新的 Calc 工作表中，然后即可保存数据或将其导出为 Calc 支持的任何文件格式。

1、打开包含要导出的数据库表格的数据库文件。点击「表格」查看表格，或点击「查询」查看查询。

2、选择「文件 - 新建 - 电子表格」。

3、在 Base 窗口中，右击要导出的表格的名称。从右键菜单中选择「复制」。

4、在新的 Calc 窗口中点击单元格 A1，然后选择「编辑 - 粘贴」。

此时即可保存数据或将其导出为多种文件类型。

#### 1.8.2 将数据导入 Base

1、打开所需数据库类型的 Base 文件。

使用Database Wizard创建一个新的 Base 文件，或者打开任何现有的非只读 Base 文件。

2、打开 Calc 文件，此文件包含要导入到 Base 的数据。您可以打开一个 *.dbf dBASE 文件或者多种其他文件类型的文件。

3、选择要复制到 Base 的数据。

如果不希望滚动，可以在名称框中输入一个类似 A1:X500 的范围引用。

如果您要复制 dBASE 工作表，请包含带有标题数据的首行。

4、选择「编辑 - 复制」。

5、在 Base 窗口中，点击「表格」以查看表格。

6、在 Base 窗口中，选择「编辑 - 粘贴」。

7、将显示「复制表格」对话框。大多数数据库都需要有一个主关键字，因此可能需要选中「创建主关键字」框。

- 注意：

  1、只能以只读模式导入文本文件、电子表格文件和系统通讯簿。

  2、从文本文件或电子表格文件导入时，该文件的首行必须包含标题信息。该文件的第二行是第一个有效数据行。第二行中每个字段的格式将确定整列的格式。电子表格文件中的所有格式信息将在导入到 Base 时丢失。

### 1.9 执行 SQL 命令

借助 SQL 命令，可以直接控制数据库，还可以建立和编辑表格与查询。

- 注意：不是所有的数据库类型都支持全部 SQL 指令。需要时请查看您的数据库系统支持的 SQL 命令。

#### 1.9.1 直接执行 SQL 语句

1、选择「文件 - 打开」可以打开数据库文件。

2、选择「工具 - SQL」。

3、点击「在 SQL 视图中创建查询」图标或从列表中选择一个查询并点击「编辑」图标。

4、在「查询」窗口中，选择「视图 - 设计视图打开/关闭」。编辑 SQL 命令。

5、点击「运行」图标. 查询结果将显示在上方的窗口中。

6、点击「保存」或「另存为」图标以保存查询。

