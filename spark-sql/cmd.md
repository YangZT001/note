spark session =》spark

## 读取文件

#### 函数

spark.read.\[ csv | format | jdbc | json | load | option | options | orc | parquet | schema   table | text | textFile \]("filePath")

#### 返回值

dataframe

------



## SQL

### 创建临时视图

#### 函数

dataframe.createOrReplaceTempView(“viewName”)

#### sql查询

spark.sql(" \*\*\*\*\*\* from viewName ")

### 创建全局临时视图

#### 函数

dataframe.createOrReplaceGlobalTempView(“viewName”)

#### sql查询

spark.sql(" \*\*\*\*\*\* from global_temp.viewName ")

------



## DSL

### 查询

dataframe.select("字段")

### 字段数据操作

dataframe.select($"字段"+1) 或

dataframe.select( ‘ 字段+1) 

**注：** 多列中有一列需要操作，则每一列都要加 **$** 或 **’** ,且不改变原数据

### 过滤filter

dataframe.filter($"字段">30)

### 分组groupBy

dataframe.groupBy("字段")

### RDD转dataframe toDF

给RDD添加字段名

rdd.toDF("字段名"...)

### dataframe转RDD rdd

dataframe.rdd()

------



## DataSet

新建样例类case class user(name:String,age:Long)

#### List创建dataSet

List(user("zhangsan",4),user("lisi",5)).toDS

### dataFrame转dataSet as

dataFrame.as[className]

### dataSet转dataFrame toDF

dataSet.toDF