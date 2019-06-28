## Welcome to the pages of my research projects

### Project1: Trajectory Analytics
[T4 - Trajectories for Traffic, Transport, and Trips](https://t4research.github.io/) is a powerful platform for analyzing different types of trajectory data, which can be applied to various applications such as Real-time Traffic Monitoring, Intelligent Traffic Signal Control and Interactive Trip Planing.

Real-time Traffic Monitoring enables intelligent analytics over real-time and historical trajectories from vehicles. At the front end, we visualize the current traffic flow and result trajectories of different types of queries. At the back end, T4 is able to support multiple types of common queries over trajectories, with compact storage, efficient index and pruning algorithms.

Intelligent Traffic Signal Control applies reinforcement learning-based traffic light controller for reducing traffic jams. We train the deep models for traffic flow prediction and traffic signal control to reduce traffic congestion.

Interactive Trip Planing enables users’ interactive exploration of POIs and trajectories in their incremental trip planning. At the back end, TISP is able to support seven types of common queries over spatial-only, spatial-textual and textual-only data, based on our proposed unified indexing and search paradigm. At the front end, we propose novel visualization designs to present the result of different types of queries.

### Project2: Visual Analytics of Geo-related multidimensional data
Both the volume and the availability of urban data related to various social issues, such as real estate, crime and population are rapidly increasing. Analysing such urban data can help the government make evidence-based decisions leading to better-informed policies; the citizens can also benefit in many scenarios such as home-seeking. However, the analytic design process can be challenging since (i) the urban data often has multiple attributes (e.g., the distance to supermarket, the distance to work, schools zone in real estate data) that are highly related to geography; and (ii) users might have various analysis/exploration tasks that are hard to define (e.g., different home-buyers might have requirements for housing properties and many of them might not know what they want before they understand the local real estate market). In this project, we use visual analytics techniques to study such geo-related multidimensional urban data and answer the following research questions. Particularly, we make the following contributions:

- We propose a visual analytics system named HomeSeekerm to help users to understand real estate markets, visually explore and compare housing properties based on their own requirements.

- We propose ConcaveCubes, a cluster-based data cube to support interactive visualization of large-scale multidimensional urban data.

- We propose AOI-shapes, to support efficient and effective visualization of user-defined urban areas of interest in an interactive manner.

**System 1 - HomeSeeker: A Visual Analytics System for Real Estate Data**

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/aIO9Y-ebLBo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>


We present an interactive visual analytics system for real estate data, named HomeSeeker, to explore the visual analytics process of geo-related multidimensional data. HomeSeeker augments existing commercial systems to help users discover hidden patterns, link various location-centred data to the price, as well as explore, filter and compare the properties, in order to easily find their preferred properties. In particular, we first present a problem abstraction for designing visualizations that help home buyers analyse real estate data. Second, we collect, integrate and clean last ten year’s real estate sold records in Australia as well as their location-related education, facility and transportation profiles, to generate a real multidimensional data repository (the dataset includes 1.42 million properties in Australia and 72 dimensions). Third, we propose an interactive visual analytic procedure to help less informed users gradually learn about the local real estate market, upon which users exploit this learned knowledge to specify their individual requirements in property seeking. Fourth, we propose a series of designs to visualize properties/suburbs in different dimensions and in different granularities. After implementing a system prototype for public access, we finally present case studies based on real-world datasets and real scenario to demonstrate the usefulness and effectiveness of our system.

*Publications*

- Li, M., Bao, Z., Sellis, T., Yan, S., & Zhang, R. (2018). HomeSeeker: A Visual Analytics System of Real Estate Data. Journal of Visual Languages & Computing, 45, 1–16. ([pdf](http://mingzhaoli.net/wp-content/uploads/2018/08/2018-HomeSeeker-A-Visual-Analytics-System-of-Real-Estate-Data.pdf)) ([demo](http://115.146.89.158/)) (ERA A)

- Li, M., Bao, Z., Sellis, T., & Yan, S. (2016). Visualization-aided exploration of the real estate data. In Australasian Database Conference (pp. 435-439). ([pdf](http://mingzhaoli.net/wp-content/uploads/2018/08/2016-HomeSeeker-Demo-ADC-2016.pdf)) (BEST DEMO AWARD)

**System 2 - ConcaveCubes: Supporting Large-scale Geographic Visualization**

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/a5a-FSleKFk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>


In this project, we study the problem of supporting effective visualization/visual analytics for large-scale geo-related multidimensional data. From an extensive literature study, we find that the existing solutions suffer from at least one of the drawbacks below: (i) loss of interesting structures/outliers due to sampling; (ii) supporting heatmaps only, which provides limited information; and (iii) no notion of real-world geography semantics (e.g., country, state, city) is captured in the visualization result as well as the underlying index. Therefore, we propose ConcaveCubes, a cluster-based data cube to support interactive visualization of large-scale multidimensional urban data. Specifically, we devise an appropriate visualization abstraction and visualization design based on clusters. We propose a novel concave hull construction method to support boundary based cluster map visualization, where real-world geographical semantics are well preserved. Instead of calculating the clusters on demand, ConcaveCubes (re)uses existing calculation and visualization results to efficiently support different kinds of user interactions. We conduct extensive experiments using real-world datasets and show the efficiency and effectiveness of ConcaveCubes by comparing with the state-of-the-art cube-based solutions.

*Publications*

- Li, M., Choudhury, F., Bao, Z., Samet, H., & Sellis, T. (2018). ConcaveCubes: Supporting Cluster-based Geographical Visualization in Large Data Scale. Computer Graphics Forum, 37(3), 217–228, 2018. ([pdf](http://mingzhaoli.net/wp-content/uploads/2018/08/2018-ConcaveCubes-EuroVis-2018.pdf)) ([video](https://www.youtube.com/watch?v=a5a-FSleKFk)) (IF: 2.046)

- Li, M., Bao, Z., Choudhury, F., & Sellis, T. (2018). Supporting Large-scale Geographical Visualization in a Multi-granularity Way. Proceedings of the Eleventh ACM International Conference on Web Search and Data Mining – WSDM ’18, 767–770. ([pdf](http://mingzhaoli.net/wp-content/uploads/2018/08/2018-li-et-al-ConvexCubes-WSDM-2018.pdf)) ([demo](http://115.146.89.158/ConcaveCubes/)) (CORE A*)

**System 3 - Interactive Visualization of Urban Areas of Interest**

<img src="https://i2.wp.com/mingzhaoli.net/wp-content/uploads/2019/06/Screenshot-2019-06-27-15.50.58.png?w=2003">

In this project, we study the problem of efficient and effective visualization of user-defined urban areas of interest. In Particular, we first describe a design space for visualizing urban AOIs based on points of interest. After extensively reviewing existing “footprint” methods, we propose a novel parameter-free footprint method, named AOI-shapes, to capture the boundary information of a user-defined urban AOI. Next, to allow interactive query refinements by the user, we propose two efficient and scalable algorithms that reuse existing visualization results to incrementally generate urban AOIs. Finally, we conduct extensive experiments with both synthetic and real-world datasets to demonstrate the effectiveness and efficiency of the proposed methods.

*Publications*

- Li, M., Bao, Z., Choudhury, F., & Sellis, T. (2019). Interactive visualization of urban areas of interest: a parameter-free and efficient footprint method. Proceedings of the Twelfth ACM International Conference on Web Search and Data Mining – WSDM ’19, 782–785. ([pdf](http://mingzhaoli.net/wp-content/uploads/2018/11/aoishapes.pdf)) (CORE A*) 

*Demo system*: http://aoishapes.com
