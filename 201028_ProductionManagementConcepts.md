# 关于生产管理的一些基本概念

## 生产管理的Life cycle

从Production order、Batch order或者kanban order的开始，到产品可以提供给顾客或者用作其他产品的生产过程所使用时为止。

## Resource

> Organization administration > Resources

创造、生产、提供商品或服务时所使用的全部的东西。例：机械、工具、人、商贩、地点……

## Resource的类型

* 仕入先（Vendor）：外部资源或者外包给其他公司。    
* 人事管理（Human Resources）：定义员工或员工group什么时候开始实行工程。   
* 機械（Machine）：使用最多的Resource类型。用它将单独的机器或机器group与Resource关联。    
* ツール（Tool）：控制、计划工具的预订量。仅在容量受限制的情况下使用。    
* 場所（Location）：控制、计划特定场所的预订。    
* 設備（Facility）：实行活动时所需的必要的建筑及固定构造。  

## リソースの能力（Resource capabilities）

> Organization administration > Resources > Resource capabilities

能力被分配给Resource。   
可以给一个Resource分配多个能力。    
可以分配一个能力给多个Resource。    

分配能力时，设定【开始日】【有效期限】，可实现Resource的临时能力。   
如果Resource的能力过期，生产时需要其能力，此时Resource无法用于生产计划。    
过期的能力可以继续被更新。   

定义生产工顺的Resource要件时，可指定多个能力作为要件。   
实行生产计划时，工顺要件定义的能力可以与Resource定义的能力互相对照。    
之后选择满足要求的Resource。    
对于多个Resource定义能力时，如果处理速度相差很大，应该区分作为不同的能力去定义。    

## 部品表（BOM，bill of materials）

> Product information management > Bill of materials and formulas > Bill of materials

制造业公司最重要的文件之一。    
生产产品之前，需要提前知道其包含什么成分、成分含量。    
BOM中记录了生产一件完成品所必要的全部的成分、零件、原材料等。    

## 工順（Route）工程（Operation）

> Production control > Operations > All routes

工顺决定产品生产时必要的流程和步骤。    
BOM定义必需的材料，Resource定义生产的地点，工顺定义从生产开始到结束一系列的事件。    

工程是生产特定产品时由工顺所组合成的任务或作业流程。    
每个任务都与完成任务所需要的时间相关联。    

## 定义可选项设定

#### 生産グループ（Production groups）

通过设定它，将production order和勘定科目相关联。    
使用勘定科目的话，可以転記order用于report，也可以将其group化。


#### 生産管理グループ（Production pools）

通过设定它，group化production order。   
处理紧急的production order，删除或転記order groups都可以实现。

#### プロパティ（Properties）

为了使用计划过程，可以给Resource定义特殊的属性。    
这些属性与working time template相联系。    

#### リソースの能力（Resource capabilities）

在多个工顺都需要Resource的情况下，创建Resource能力。    
上述情况可以用Resource能力的set来表示。   
由此，Resource的分配可以延期到生产计划时。   

## 生产的Life cycle和Status

作成（Create）    
見積（Estimate）    
スケジュール（Schedule）    
リリース（Released）    
開始（Start）   
完了レポート（Report as finished）    
終了（End）

### 参考资料

[https://docs.microsoft.com/en-us/learn/modules/get-started-production-control-dyn365-supply-chain-mgmt/2-concepts-prod-control](https://docs.microsoft.com/en-us/learn/modules/get-started-production-control-dyn365-supply-chain-mgmt/2-concepts-prod-control)
