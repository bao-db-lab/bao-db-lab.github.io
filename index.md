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
