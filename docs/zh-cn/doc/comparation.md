# 其他方案对比

- **方案1. 常备多套测试环境**

**优点**：环境随时可用

**缺点**：治标不治本，太多项目并行依然会不够用；无人使用时产生数倍资源浪费；额外的资源分配和管理问题

- **方案2. 用helm等工具“快速”创建一套环境，用完就删**

**优点**：空闲时资源浪费最少

**缺点**：批量拉起所有服务，整个环境就绪等待时间可能长达几分钟到几十分钟；有时候为了测试一个服务拉一套环境，运行时资源消耗高；完整的环境不但需要启动服务，还要导入各个服务的数据，带来数据和脚本维护成本