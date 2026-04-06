Parallelism in computer science refers to the simultaneous execution of multiple tasks using multiple processors or cores. There are several different forms of parallel computing: bit-level, instruction-level, data, and task parallelism. Parallelism has long been employed in high-performance computing but has gained broader interest due to the physical constraints preventing frequency scaling.

## Pipelines

A task pipeline is a collection of tasks that are defined and arranged in a specific order of execution as part of a continuous integration flow. Each task in a pipeline performs an action, such as building an app, interacting with resources, installing a tool, or running a test. Tasks are the building blocks for defining automation in a pipeline.

[(2) Azure Pipelines task reference | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/reference/?view=azure-pipelines) 
[(3) Build and Release Tasks - Azure Pipelines | Microsoft Learn](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/tasks?view=azure-devops )

![[parallelism.png]]
Sometimes tasks can be started at the same time as long as they are independent of each other. Other tasks have a dependency on another one. The whole process for everything from start to finish is called the "pipeline".

## Critical Path
The critical path refers to the sequence or order of scheduled activities that will make up the entire duration of a project. It represents the longest path through the entirety of the project and typically this path consists of every single activity that must be concluded from the kickoff to the ultimate conclusion of the project¹. The critical path method is a technique that allows you to identify tasks that are necessary for project completion³.

[(1) Critical Path - Project Management Knowledge](https://project-management-knowledge.com/definitions/c/critical-path/ )
[(2) Critical path method: How to use CPM for project management](https://asana.com/resources/critical-path-method)
[(3) What Is Critical Path? A Comprehensive Guide 2023 | PM]( https://project-management.com/what-is-critical-path/ )

You can optimize pipelines in more than one way to increase the speed at which you complete tasks.

## Latency

**latency** refers to the time it takes for a system to respond to a given input
- How much time does it take to process data?
- *How long is the pipe?*

You can improve your latency by:
- Removing unnecessary tasks
- Shorten tasks, i.e. complete them faster or shorten waiting time.

Eventually, the amount of effort spent in improving a particular task is not worth the investment in tackling the complexity of the improvements or optimizations.

> Bottlenecks are the core problem of latency

## Throughput

**Throughput** refers to the rate at which a system can process inputs.
- How much data can be processed at once?
- *How wide is the pipe?*

You can improve your throughput:
- Adding more resources to completing tasks
- Optimizing resource usage to reduce idle time

Eventually, adding more resources will not add enough additional value to justify their costs. 

> 9 women cannot create a baby in 1 month.