---
layout: posts
title: What matters for AI cloud services
duration: 15
category: Machine Learning, Business
tags: [deep learning, machine learning, business]
comments: true
---

Any technology that is algorithmic can be offered as a service using the cloud. What then governs whether the cloud is the right approach for developing new products built on algorithmic technology? I believe that evaluation on the following metrics are crucial to the success of a cloud API based implementation:

- functional latency
- implementation complexity
- development agility
- scope scalability

One quickly realized that such products are marketed and built for software developers. They are the customers. These are intended to make their lives easier. These are intended to make them more effective at what they do. In my experience as a software developer, people are often wowed by the results of what you do and less so by the techniques that you followed to produce those results. Cloud vs local is a function of methodology and if a developer can produce results faster, allow for quick tuning and enable better forms of abstraction of algorithmic components, that allows others to understand the methodology and results equally well. Moreover, cloud API forces you to think about algorithms in a modular manner because you are fundamentally constrained by the granularity of the API call. The most detailed explanation of a cloud-based algorithm is based on a thorough description of the lowest level API calls made in the implementation.
Very often the success of AI-based technologies and ML solutions is more a function of a good mapping of product-to-problem and a strong understanding of the data used to train and predict the ML algorithm than the innovation at the algorithmic level. Cloud APIs will provide the tools in a ML software developers arsenal that allows them to be creative and work to develop and manipulate with a deeper understanding of the data involved to solve for a specific problem. Today, AMZN has a leg up over the competition at comprehensiveness, MSFT has an advantage on enterprise and tools integration. GOOG is pitching an advantage on ML algorithmic superiority and effectiveness.

One can make the argument that their is need to making a choice. Go with what works at the right time in your development cycle by avoiding PaaS lock-in. The reality is that multiple vendors have been trying to develop AI and ML based cloud solutions. [Google] with their sentiment and speech recognition API are trying to own a unique position in this space. They face competition from AMZN’s Dstny API, MSFT’s [ML Studio] and IBM’s [Watson Analytics]. GOOG has been pitching the open source nature and community support and intellectual aggregation in TensorFlow coupled with the speed of implementation on the [TensorFlow processor] as a unassailable advantage on implementing cloud-based AI algorithms. Over time, however, the cloud APIs will be democratized. Algorithmic and platform level strengths are weaker than hardware based differentiation. Over time, the real pitch to any developer or development team or solution provider (let’s just call them product entity) would be a holistic cloud service that can be optimized for their specific use case. I feel that this approach has been instrumental toward the success of AMZN and will be central to the success of any cloud based solution provider. Unlike hardware based solutions, product entities are less attached to any one solution provider. In the early days, product entities use and try different solutions to better understand what works for them. Over time as product entities scale on their number of users/customers and on the requirements and comprehensiveness of their offerings, their needs for a cloud API change. This would encourage them to “shop” more frequently and be less attached to any one solution that they have tried before. To add to their convenience, there is tremendous growth in the use of containerized services like Docker and Mesos to enable easier transition between different cloud API services.

Unbundling/Fragmentation:

Containerization and container orchestration frameworks allow for worthy substitute to PaaS options like AMZN AWS/GOOG Cloud/MSFT Azure/Digital Ocean. This allows for custom implementations. Couple of arguments used in the favor of this approach are the following (inspired by [Denny Britz]):

- Costs: Fixed + Pay-Per-Use model of AWS vs close to free pricing for containerized applications + cloud charges
- Features: Some developers cite the fact that AWS is often based on open source projects forked for integration into the PaaS. The counterargument to this limitation is that this approach makes sense to the PaaS provider as it allows for better maintainability and stability of their offering. Also, key features that are of demand by users/product entities can be integrated into future releases of the PaaS solution. Need-based feature staging can be a beneficial approach to these cloud PaaS vendors. Product entities tend to use cloud PaaS for meaningful abstractions of cloud services and mostly prefer to focus on application development rather than debugging PaaS components
- Cloud-lock in: agreed! this is a long/short term benefit
- Control: Product entities need to rely on cloud PaaS to support new features and fix bugs while using open source containerized applications can allow for “faster” (if approached by the right development resources) debugging on bleeding edge open source projects. But really, once a product entity invests a significant amount of time early on for a containerized implementation of bleeding edge software components, it is unlikely to release them back to the community through a hosting like DockerHub.

[Google]: http://www.theverge.com/2016/7/22/12255334/google-cloud-ai-deepmind?yptr=yahoo
[TensorFlow chip]: http://www.theverge.com/circuitbreaker/2016/5/19/11716818/google-alphago-hardware-asic-chip-tensor-processor-unit-machine-learning
[ML Studio]: http://www.kdnuggets.com/2014/11/microsoft-azure-machine-learning.html
[Watson Analytics]: http://www.kdnuggets.com/2014/12/ibm-watson-analytics-microsoft-azure-machine-learning-p1.html
[Denny Britz]: http://blog.dennybritz.com/2015/10/06/the-unbundling-of-aws/
