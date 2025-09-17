# Heythem SATTOUTAH

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/haithem-satoutah/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/satoutahhaithem)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0004-0258-3446)

## About Me

I am a Computer Science Engineer specializing in computer networks, security, machine learning, and robotics. I hold a Master’s degree in Computer Networks from Sorbonne University in Paris, building on a strong academic foundation from the Higher School of Computer Science (ESI SBA) in Algeria. My expertise spans network infrastructure, quality of service optimization, and solving complex computational problems.

I recently completed an R&D internship at Renault Ampere, where I worked on multi-agent connectivity and clustering solutions. My professional experience also includes contributions in data center environments, database management, and network topology implementation at major companies such as Sonatrach.

My research interests focus on optimization problems, particularly the use of Maximum Satisfiability (Max-SAT) approaches for solving p-center and p-median location problems, with applications in bioinformatics and planning. I am passionate about applying theoretical computer science to real-world challenges, bridging innovation in research with impactful engineering solutions.

## Table of Contents

- [Projects](#projects)
  - [Quality of Service Implementation](#quality-of-service-implementation)
  - [Remote Robot Control System](#remote-robot-control-system-with-video-surveillance-and-object-detection-capabilities)
  - [AI Cluster for Home Devices](#ai-cluster-for-home-devices)
  - [Distributed Computing Cluster Configuration](#distributed-computing-cluster-configuration)
  - [P-Center Location Problem](#p-center-location-problem)
  - [Scheduling Problem Optimization](#scheduling-problem-optimization)
  - [Final Year Projects Management System](#final-year-projects-management-system)
  - [Attendance Verification Application](#attendance-verification-application)
  - [BMI Application (Java/Android)](#bmi-application-javaandroid)
- [Publications](#publications)
  - [Maximum Satisfiability Approach for P-Center and P-Median Location Problems](#maximum-satisfiability-approach-for-p-center-and-p-median-location-problems)
  - [Constraint Programming Approaches for Location Problems](#constraint-programming-approaches-for-location-problems)
- [Contact](#contact)

## Projects

### Quality of Service Implementation
*Network Engineering Project*

This project focuses on implementing and optimizing Quality of Service (QoS) mechanisms in network environments to ensure efficient resource allocation, prioritization of critical traffic, and consistent performance for diverse applications.

**Technical Foundation:**
The implementation is built on a comprehensive understanding of QoS principles and technologies:

- **Traffic Classification**: Developed sophisticated methods for identifying and categorizing network traffic based on:
  - Application signatures and behavior patterns
  - Protocol characteristics
  - Source/destination attributes
  - Content type and business priority

- **Policy Framework**: Created a flexible policy definition system that allows for:
  - Hierarchical policy structures with inheritance
  - Time-based policy activation
  - Dynamic policy adjustment based on network conditions
  - Exception handling for special cases

- **Implementation Mechanisms**: Utilized multiple complementary QoS techniques:
  - Traffic shaping using token bucket algorithms
  - Class-based weighted fair queuing
  - Low latency queuing for delay-sensitive applications
  - Random Early Detection (RED) for congestion management
  - DSCP marking for end-to-end QoS coordination

**Project Components:**
The project consists of several integrated components:

1. **Traffic Analysis Module**: 
   - Deep packet inspection capabilities
   - Flow-based traffic analysis
   - Application recognition engine
   - Traffic pattern visualization

2. **Policy Management System**:
   - Web-based policy configuration interface
   - Policy validation and conflict detection
   - Version control for policy changes
   - Policy simulation for impact analysis

3. **Enforcement Engine**:
   - High-performance packet processing
   - Hardware acceleration integration
   - Real-time queue management
   - Adaptive bandwidth allocation

4. **Monitoring and Reporting**:
   - Real-time performance dashboards
   - Historical trend analysis
   - SLA compliance reporting
   - Anomaly detection and alerting

**Implementation Scenarios:**
The QoS framework was tested and optimized for several critical use cases:

1. **Enterprise WAN Optimization**:
   - Prioritization of business-critical applications
   - VoIP and video conferencing quality assurance
   - Bandwidth management for large file transfers
   - Cloud application performance optimization

2. **Data Center Traffic Management**:
   - Storage network traffic isolation
   - Inter-server communication optimization
   - Backup traffic deprioritization
   - Management traffic protection

3. **Service Provider Edge**:
   - Customer SLA enforcement
   - Traffic policing at network boundaries
   - Hierarchical QoS for multi-tenant environments
   - Congestion management during peak periods

**Repositories**:
- [Quality-of-Service](https://github.com/satoutahhaithem/Quality-of-Service): Core implementation of QoS mechanisms and policies
- [traffic-shapping_tasks](https://github.com/satoutahhaithem/traffic-shapping_tasks): Specialized traffic shaping implementations and testing scenarios

### Remote Robot Control System with Video Surveillance and Object Detection Capabilities
*Academic Project | February 2023 - June 2023*

This project represents a significant advancement in remote robotics control systems, combining real-time video surveillance with sophisticated object detection capabilities. The system was designed to address the growing need for autonomous and semi-autonomous robotic systems that can operate in various environments while providing real-time feedback and intelligent decision-making capabilities.

**Technical Implementation:**
The architecture integrates multiple cutting-edge technologies to create a cohesive and powerful system:

- **Machine Learning Integration**: The project implements advanced machine learning algorithms that enable the robot to detect and classify objects in real-time. Using computer vision techniques and neural networks, the system can identify various objects, determine their positions, and make decisions based on this information. This capability is crucial for applications in security, industrial automation, and research environments where object recognition is essential.

- **Big Data Processing**: A key innovation in this project is the integration of Apache Kafka for handling the large volumes of data generated during operation. The streaming platform manages video feeds, sensor data, and command signals efficiently, ensuring minimal latency and reliable data transmission between the robot and control systems. This big data approach allows for scalable performance even when processing high-definition video streams and complex sensor inputs simultaneously.

- **Dual-Mode Operation**: The system was engineered to function in both standalone and server-connected modes:
  - In standalone mode, the robot operates independently using onboard processing capabilities
  - In server mode, it connects to more powerful computing resources for enhanced processing capabilities and remote monitoring

- **Containerization with Docker**: The entire system is containerized using Docker, which provides several advantages:
  - Consistent deployment across different environments
  - Simplified dependency management
  - Improved collaboration through standardized development environments
  - Enhanced scalability for adding additional robots or processing nodes

**Challenges and Solutions:**
One of the primary challenges was optimizing the real-time video processing while maintaining low latency for control commands. This was addressed through:

1. Implementing efficient video compression algorithms
2. Creating a prioritized message queue system in Kafka
3. Developing a custom protocol for command transmission that minimizes overhead

Another significant challenge was ensuring reliable operation in environments with unstable network connections. The solution involved:

1. Creating a robust fallback mechanism for the robot to operate autonomously when connection is lost
2. Implementing a data buffering system to prevent information loss during connectivity issues
3. Developing a reconnection protocol that seamlessly transitions between standalone and server modes

**Repository**: [Live-Streaming-From-Raspberry-to-pc-Using-Kafka-broker](https://github.com/satoutahhaithem/Live-Streaming-From-Raspberry-to-pc-Using-Kafka-broker)

### AI Cluster for Home Devices
*System Integration Project*

This project represents an innovative approach to distributed artificial intelligence by enabling everyday consumer devices to form a cohesive AI computing cluster. Based on the Exo framework, this implementation allows smartphones, computers, IoT devices, and other consumer electronics to contribute their computational resources to AI workloads that would typically require specialized hardware.

**Technical Foundation:**
The system builds upon the Exo project with several custom enhancements:

- **Device Discovery and Integration**: Implemented protocols for:
  - Automatic detection of compatible devices on local networks
  - Capability assessment and resource profiling
  - Secure pairing and authentication
  - Dynamic join/leave handling

- **Workload Distribution**: Developed intelligent task allocation mechanisms:
  - Device-specific task optimization
  - Adaptive load balancing based on device capabilities
  - Power-aware scheduling for mobile devices
  - Fault tolerance with task migration

- **Resource Management**: Created systems for efficient utilization:
  - Dynamic resource allocation based on device state
  - Background processing prioritization
  - Thermal management integration
  - Battery-aware operation for mobile devices

- **Network Optimization**: Implemented efficient communication:
  - Bandwidth-aware data transfer
  - Compression for resource-constrained connections
  - Local caching to reduce redundant transfers
  - Mesh networking for device-to-device communication

**Key Innovations:**
The project introduces several novel approaches to distributed AI:

1. **Heterogeneous Device Integration**:
   - Support for diverse computational architectures (ARM, x86, RISC-V)
   - Hardware acceleration detection and utilization (GPU, NPU, DSP)
   - Adaptive algorithm selection based on available hardware
   - Cross-platform code execution environment

2. **Edge-Optimized AI Models**:
   - Model partitioning for distributed inference
   - Progressive model loading based on device capabilities
   - Quantization and optimization for resource-constrained devices
   - Federated learning implementation for privacy-preserving training

3. **Resilient Operation**:
   - Graceful degradation with device disconnection
   - State synchronization for consistent operation
   - Checkpoint/restore for long-running tasks
   - Power failure recovery mechanisms

4. **User Experience Integration**:
   - Minimal impact on device primary functions
   - Intuitive cluster management interface
   - Real-time contribution visualization
   - Participation incentive system

**Application Scenarios:**
The system enables several compelling use cases for home AI deployment:

1. **Distributed Smart Home Intelligence**:
   - Coordinated processing across multiple smart home devices
   - Privacy-preserving local processing of sensitive data
   - Enhanced response times compared to cloud-based alternatives
   - Continued operation during internet outages

2. **Collaborative Content Creation**:
   - Distributed rendering for 3D projects
   - Multi-device video processing
   - Shared computational photography enhancements
   - Collaborative AI-assisted design

3. **Personal AI Research**:
   - Accessible platform for AI experimentation
   - Reduced dependency on cloud computing resources
   - Custom model training on personal data
   - Educational tool for distributed systems concepts

The project demonstrates how consumer devices can collectively provide significant AI computing capabilities without dedicated hardware investments, democratizing access to advanced AI applications.

**Repository**: [exo](https://github.com/satoutahhaithem/exo) (Forked from exo-explore/exo)

### Distributed Computing Cluster Configuration
*System Administration Project*

This project focuses on the design, implementation, and optimization of distributed computing clusters for high-performance computing applications. The work addresses the complex challenges of creating efficient, scalable, and resilient computational environments for resource-intensive tasks.

**Technical Architecture:**
The cluster configuration implements a comprehensive approach to distributed computing:

- **Node Management**: Developed sophisticated scripts and configurations for:
  - Automated node provisioning and configuration
  - Health monitoring and failure detection
  - Dynamic resource allocation
  - Heterogeneous hardware integration

- **Network Infrastructure**: Optimized for high-throughput, low-latency communication:
  - InfiniBand fabric configuration for high-speed inter-node communication
  - Network topology optimization for minimizing hop counts
  - Traffic segregation for different communication patterns
  - Redundant paths for fault tolerance

- **Storage Systems**: Implemented distributed storage solutions:
  - Parallel file systems for high-throughput I/O
  - Tiered storage with SSD caching
  - Data locality optimization
  - Backup and disaster recovery mechanisms

- **Job Scheduling**: Configured advanced workload management:
  - Fair-share scheduling policies
  - Resource reservation capabilities
  - Job dependency management
  - Priority-based preemption

**Implementation Details:**
The project includes several key components implemented through shell scripting, configuration management, and system administration techniques:

1. **Cluster Bootstrapping**:
   - Automated PXE boot environment
   - Configuration management with Ansible
   - Node image creation and distribution
   - Post-installation validation

2. **Performance Optimization**:
   - CPU frequency scaling and governor configuration
   - Memory management tuning
   - Network buffer optimization
   - I/O scheduler selection and configuration

3. **Monitoring and Management**:
   - Comprehensive metrics collection
   - Real-time performance visualization
   - Alerting and notification system
   - Historical performance analysis

4. **Security Implementation**:
   - Network isolation and segmentation
   - Authentication and authorization framework
   - Audit logging and compliance reporting
   - Secure communication channels

**Use Cases and Applications:**
The cluster configuration has been optimized for several demanding computational workloads:

1. **Scientific Computing**:
   - Physics simulations
   - Genomic sequence analysis
   - Climate modeling
   - Computational chemistry

2. **Data Analytics**:
   - Large-scale data processing
   - Machine learning model training
   - Graph analytics
   - Real-time stream processing

3. **Rendering and Visualization**:
   - 3D rendering farms
   - Scientific visualization
   - Video transcoding
   - Image processing pipelines

The project demonstrates how careful system configuration and optimization can significantly improve computational efficiency, resource utilization, and overall cluster performance for diverse workloads.

**Repository**: [Config_distributed_cluster](https://github.com/satoutahhaithem/Config_distributed_cluster)

### P-Center Location Problem
*Research Project*

This research project addresses the p-center location problem, a fundamental challenge in facility location theory with significant practical applications in emergency service placement, telecommunications network design, and public infrastructure planning.

**Problem Definition and Significance:**
The p-center problem involves locating p facilities to minimize the maximum distance between any demand point and its nearest facility. This minimax objective is particularly relevant in emergency service contexts where the worst-case response time is critical. The problem is known to be NP-hard, making efficient solution approaches for large instances particularly valuable.

**Research Approach:**
This project explores a novel approach to solving p-center problems using Maximum Satisfiability (Max-SAT) techniques. The methodology includes:

1. **Problem Transformation**: Developing a systematic approach to transform p-center problems into equivalent Max-SAT formulations, enabling the use of state-of-the-art SAT solvers

2. **Algorithm Development**: Creating specialized algorithms that exploit the structure of p-center problems when represented in Boolean logic

3. **Comparative Analysis**: Conducting extensive computational experiments comparing the Max-SAT approach against traditional methods including:
   - Greedy algorithms
   - Linear programming relaxations
   - Metaheuristic approaches
   - The Calik algorithm (a leading approach in the literature)

**Technical Implementation:**
The project implementation includes several sophisticated components:

- **Encoding Framework**: A flexible system for transforming various p-center problem variants into CNF formulas suitable for Max-SAT solvers

- **Custom Solver Extensions**: Modifications to existing Max-SAT solvers to incorporate domain-specific knowledge about location problems

- **Instance Generator**: Tools for creating synthetic problem instances with controlled properties to systematically evaluate algorithm performance

- **Visualization Module**: Geographic visualization of solution quality, showing facility placements and coverage areas

**Research Findings:**
The project has yielded several significant findings:

1. The Max-SAT approach demonstrates superior performance for certain classes of p-center problems, particularly those with specific structural properties

2. For large-scale instances, hybrid approaches combining initial solutions from greedy algorithms with Max-SAT refinement provide the best balance of solution quality and computational efficiency

3. The Boolean logic representation enables more effective handling of additional constraints that are challenging to incorporate in traditional mathematical programming formulations

4. Detailed analysis of algorithm behavior has revealed insights into the landscape of p-center problems that can guide future algorithm development

**Repositories**:
- [max-sat_p-center](https://github.com/satoutahhaithem/max-sat_p-center): Implementation of the Max-SAT approach for p-center problems
- [Calik-p-center_Tests](https://github.com/satoutahhaithem/Calik-p-center_Tests): Comparative analysis with the Calik algorithm, a benchmark approach in the literature

### Scheduling Problem Optimization
*Research Project*

This comprehensive research project explores advanced approaches to solving complex scheduling problems through various optimization techniques. Scheduling problems represent a critical area in operations research with applications spanning manufacturing, healthcare, transportation, and computing resource allocation.

**Project Scope and Methodology:**
The project investigates multiple algorithmic approaches to scheduling optimization, with a particular focus on:

- **Constraint Programming Models**: Developing formal constraint satisfaction models that accurately represent complex scheduling requirements including resource constraints, precedence relationships, and time windows
  
- **Mathematical Optimization**: Implementing mixed-integer linear programming formulations to find optimal solutions for scheduling problems of moderate size

- **Metaheuristic Approaches**: Creating and evaluating specialized algorithms including genetic algorithms, simulated annealing, and tabu search for larger problem instances where exact methods become computationally prohibitive

- **Hybrid Methods**: Combining exact and approximate methods to leverage the strengths of both approaches, particularly for problems with specific structural properties

**Implementation Details:**
The project includes several key components:

1. **Problem Instance Generator**: A customizable tool for creating diverse scheduling problem instances with varying characteristics to thoroughly test algorithm performance

2. **Algorithm Library**: Implementation of multiple solution approaches in Python, with integration to specialized solvers including:
   - IBM CPLEX for mathematical programming models
   - OR-Tools for constraint programming formulations
   - Custom metaheuristic implementations

3. **Benchmarking Framework**: A comprehensive system for evaluating algorithm performance across multiple metrics:
   - Solution quality (makespan, tardiness, resource utilization)
   - Computational efficiency (runtime, memory usage)
   - Scalability with problem size

4. **Visualization Tools**: Interactive visualizations for schedule representation, resource allocation, and algorithm convergence analysis

**Research Contributions:**
This project makes several notable contributions to the field of scheduling optimization:

1. Identification of problem-specific heuristics that significantly improve solution quality for certain classes of scheduling problems

2. Development of novel hybrid algorithms that outperform traditional approaches on benchmark instances

3. Comprehensive empirical analysis comparing different modeling approaches and their suitability for various problem characteristics

4. Implementation of practical scheduling solutions that can be applied to real-world industrial and organizational contexts

**Repositories**:
- [ROADEF_SCHEDULING](https://github.com/satoutahhaithem/ROADEF_SCHEDULING): Implementation focused on the ROADEF challenge scheduling problems
- [Scheduling_Problem_JFPC](https://github.com/satoutahhaithem/Scheduling_Problem_JFPC): Specialized algorithms presented at the French Conference on Constraint Programming
- [Ceplex_Python_Roadef_Scheduling](https://github.com/satoutahhaithem/Ceplex_Python_Roadef_Scheduling): Integration of CPLEX solver with Python for advanced scheduling optimization

### Final Year Projects Management System
*Academic Project | February 2022 - June 2022*

This project addressed the complex challenge of managing final year academic projects within educational institutions. The system provides a comprehensive digital platform that streamlines the entire project lifecycle from proposal to final evaluation.

**System Architecture:**
The application follows a modern full-stack architecture:

- **Frontend**: Developed with React.js, providing a responsive and intuitive user interface with:
  - Dynamic dashboard views customized for different user roles
  - Real-time notification system for important deadlines and updates
  - Interactive project timeline visualization
  - Document management interface with version control

- **Backend**: Built on Laravel PHP framework, implementing:
  - RESTful API architecture for seamless frontend-backend communication
  - Role-based access control system with fine-grained permissions
  - Automated scheduling and reminder system
  - Comprehensive reporting and analytics engine

- **Database**: Structured relational database with optimized schema design for:
  - Efficient storage of project metadata, submissions, and evaluations
  - Maintaining historical records for institutional knowledge preservation
  - Supporting complex queries for reporting and analysis

**Key Features:**
The system includes several innovative features designed to address specific challenges in academic project management:

1. **Project Lifecycle Management**:
   - Structured workflow from proposal submission to final defense
   - Milestone tracking with automated notifications
   - Document repository with version control and access permissions

2. **Supervisor-Student Collaboration**:
   - Communication platform with threaded discussions
   - Meeting scheduling and minutes recording
   - Progress tracking with customizable metrics

3. **Evaluation Framework**:
   - Configurable rubrics for different project types
   - Multi-evaluator support with conflict resolution
   - Plagiarism detection integration
   - Statistical analysis of evaluation patterns

4. **Resource Allocation**:
   - Intelligent matching of students to supervisors based on expertise and interests
   - Laboratory and equipment reservation system
   - Budget tracking for funded projects

**Implementation Challenges:**
Several technical challenges were addressed during development:

1. Creating a scalable architecture capable of handling peak loads during submission deadlines
2. Implementing a secure document handling system with appropriate access controls
3. Designing an intuitive interface that accommodates users with varying levels of technical proficiency
4. Ensuring data integrity across the complex relationships between projects, users, and evaluations

The system has significantly improved the efficiency of project management processes, reducing administrative overhead and providing valuable insights through its analytics capabilities.

### Attendance Verification Application
*Academic Project | February 2021 - June 2021*

This project involved the development of a comprehensive mobile and web application for tracking and verifying attendance in educational and professional settings. The system provides an efficient alternative to traditional paper-based attendance methods, offering real-time tracking, reporting, and analytics.

**Technical Architecture:**
The application was built using a modern cross-platform approach:

- **Mobile Frontend**: Developed with Flutter, providing:
  - Native-like performance on both Android and iOS
  - Offline functionality with data synchronization
  - Biometric authentication options
  - QR code scanning capabilities for quick check-in

- **Web Backend**: Implemented using Laravel, featuring:
  - RESTful API architecture
  - Robust authentication and authorization
  - Comprehensive data validation
  - Efficient database operations

- **Database Design**: Structured to support:
  - Complex attendance patterns and schedules
  - Hierarchical organizational structures
  - Historical data analysis
  - Performance optimization for large datasets

**Key Features:**
The application includes several innovative features designed to address common challenges in attendance management:

1. **Multiple Verification Methods**:
   - QR code-based check-in/check-out
   - Geolocation verification with configurable boundaries
   - Biometric verification options
   - PIN/password backup methods

2. **Flexible Scheduling System**:
   - Support for regular and irregular schedules
   - Holiday and exception handling
   - Time zone management for distributed teams
   - Shift pattern definitions

3. **Comprehensive Reporting**:
   - Real-time attendance dashboards
   - Customizable report generation
   - Attendance pattern analysis
   - Exportable reports in multiple formats

4. **Integration Capabilities**:
   - API for third-party system integration
   - Data import/export functionality
   - Calendar synchronization
   - Notification system integration

**Implementation Challenges:**
Several technical challenges were addressed during development:

1. Ensuring reliable operation in environments with intermittent connectivity
2. Implementing secure verification methods resistant to spoofing
3. Optimizing battery usage for mobile location tracking
4. Creating an intuitive interface suitable for users with varying technical proficiency

The application has been successfully deployed in educational settings, demonstrating significant improvements in attendance tracking efficiency and accuracy compared to traditional methods.

**Repository**: [Tp4-Dev-Mobile-Note-Application](https://github.com/satoutahhaithem/Tp4-Dev-Mobile-Note-Application)

### BMI Application (Java/Android)
*Mobile Development Project*

This project involved the development of a comprehensive Body Mass Index (BMI) calculator application for Android devices. While seemingly straightforward, the application incorporates sophisticated features that go beyond basic BMI calculation to provide users with a holistic health assessment tool.

**Technical Implementation:**
The application was developed using Java for Android, employing a clean architecture approach:

- **User Interface Layer**: Designed with Material Design principles for intuitive interaction:
  - Responsive layouts adapting to different screen sizes
  - Animated transitions for enhanced user experience
  - Accessibility features for users with disabilities
  - Dark mode support for reduced eye strain

- **Business Logic Layer**: Implemented comprehensive health assessment algorithms:
  - BMI calculation with age and gender adjustments
  - Body fat percentage estimation
  - Basal Metabolic Rate (BMR) calculation
  - Daily caloric needs estimation

- **Data Persistence Layer**: Created for tracking progress over time:
  - Local SQLite database for measurement history
  - Data export functionality for sharing with healthcare providers
  - Secure storage of sensitive health information
  - Backup and restore capabilities

**Key Features:**
The application includes several features that distinguish it from typical BMI calculators:

1. **Comprehensive Measurement Options**:
   - Support for both metric and imperial units
   - Multiple measurement methods (height/weight, waist/hip ratio)
   - Body frame size adjustment
   - Age and gender-specific calculations

2. **Visual Result Interpretation**:
   - Color-coded BMI category indicators
   - Interactive BMI scale visualization
   - Comparison to population averages
   - Trend analysis with historical data

3. **Personalized Recommendations**:
   - Health risk assessment based on BMI and other factors
   - Customized weight management suggestions
   - Activity level recommendations
   - Nutritional guidance based on calculated metrics

4. **Progress Tracking**:
   - Timeline visualization of BMI changes
   - Goal setting and milestone tracking
   - Statistical analysis of progress
   - Reminder system for regular measurements

**Development Challenges:**
Several technical challenges were addressed during implementation:

1. Ensuring calculation accuracy across different measurement systems and edge cases
2. Creating an intuitive interface that presents complex health information in an accessible manner
3. Implementing efficient data storage and retrieval for historical tracking
4. Balancing comprehensive features with application performance on lower-end devices

The application serves as both a practical health tool for users and a demonstration of Android development best practices, including responsive design, efficient data management, and intuitive user experience.

**Repository**: [Bmi-Application-java-android](https://github.com/satoutahhaithem/Bmi-Application-java-android)

## Publications

### Maximum Satisfiability Approach for P-Center and P-Median Location Problems
*Publication at JFPC (French Conference on Constraint Programming), 2024*

This research paper introduces a novel approach to solving the classical p-center and p-median location problems using Maximum Satisfiability (Max-SAT) techniques. Location problems represent a fundamental class of optimization challenges with applications spanning emergency service placement, telecommunications infrastructure, retail location planning, and public facility distribution.

**Research Contributions:**

The paper makes several significant contributions to the field:

1. **Novel Problem Formulation**: The research presents a systematic transformation of p-center and p-median problems into Boolean satisfiability instances, enabling the application of state-of-the-art SAT solvers to these traditionally graph-theoretical problems.

2. **Algorithm Development**: The paper introduces specialized algorithms that exploit the structure of location problems when represented in Boolean logic, including:
   - Custom encoding techniques that reduce formula size
   - Problem-specific preprocessing methods
   - Specialized branching heuristics for the SAT solving process

3. **Theoretical Analysis**: The work provides formal proofs regarding:
   - The correctness of the transformation
   - Complexity analysis of the resulting SAT instances
   - Bounds on solution quality for approximate approaches

4. **Empirical Evaluation**: Comprehensive computational experiments demonstrate:
   - Superior performance on certain problem classes compared to traditional approaches
   - Scaling characteristics with problem size
   - Sensitivity analysis to various problem parameters
   - Comparative analysis with state-of-the-art methods

**Methodology:**

The research methodology combines theoretical development with rigorous empirical validation:

1. The paper begins by establishing a formal framework for representing location problems as Max-SAT instances, with particular attention to encoding efficiency.

2. Several algorithmic enhancements are proposed to improve solver performance on the resulting instances, including specialized preprocessing techniques and custom branching heuristics.

3. A comprehensive benchmark suite is developed, incorporating both standard test instances from the literature and new challenging cases designed to test specific aspects of the approach.

4. Extensive computational experiments are conducted to evaluate the approach against leading methods from the literature, with detailed analysis of performance characteristics.

**Impact and Applications:**

The research has significant implications for both theoretical understanding and practical applications:

1. **Theoretical Advancement**: The work establishes new connections between combinatorial optimization and Boolean satisfiability, potentially opening avenues for cross-fertilization between these fields.

2. **Practical Applications**: The improved solution methods enable more effective facility location in various domains:
   - Emergency service placement with improved worst-case response times
   - Telecommunications network design with optimized coverage
   - Public infrastructure planning with enhanced accessibility

3. **Computational Efficiency**: For certain problem classes, the approach provides solutions to previously intractable instances, expanding the practical applicability of location optimization.

This publication represents a significant contribution to the field of combinatorial optimization, introducing novel techniques that bridge the gap between location theory and Boolean satisfiability research.

### Constraint Programming Approaches for Location Problems
*Publication at CP (International Conference on Constraint Programming) in Spain, 2024*

This research paper extends the investigation of location problems through the lens of constraint programming (CP), building upon the Max-SAT approach presented at JFPC. The work explores how the rich modeling capabilities and specialized propagation techniques of constraint programming can be leveraged to solve complex location problems more effectively.

**Research Contributions:**

The paper makes several notable contributions to the field:

1. **Expressive Modeling Framework**: The research develops a comprehensive constraint programming model for location problems that can naturally incorporate complex side constraints often encountered in real-world scenarios, such as:
   - Capacity limitations
   - Budget constraints
   - Incompatibility between facilities
   - Hierarchical service requirements
   - Backup coverage requirements

2. **Global Constraints**: The paper introduces specialized global constraints for location problems that encapsulate common substructures and enable more efficient propagation:
   - A custom covering constraint that efficiently handles radius-based coverage
   - A facility interaction constraint that manages relationships between co-located facilities
   - A balanced assignment constraint that ensures equitable distribution of demand

3. **Hybrid Solution Methods**: The work presents innovative hybrid approaches that combine:
   - Constraint programming for handling complex constraints
   - Linear programming relaxations for bound computation
   - Local search for solution refinement
   - Learning-based search strategies that adapt to problem characteristics

4. **Benchmark Results**: Comprehensive computational experiments demonstrate:
   - The effectiveness of the constraint programming approach on complex instances
   - Performance comparison with traditional mathematical programming methods
   - Analysis of the impact of different modeling choices and search strategies
   - Scaling behavior with problem size and constraint complexity

**Methodology:**

The research methodology combines theoretical modeling with algorithm development and empirical validation:

1. The paper begins by developing a general constraint programming framework for location problems, with particular attention to modeling flexibility and propagation efficiency.

2. Several specialized global constraints are designed and implemented, with formal analysis of their filtering strength and computational complexity.

3. Hybrid solution strategies are developed that leverage the complementary strengths of different optimization paradigms, with mechanisms for information exchange between components.

4. A comprehensive experimental evaluation is conducted on both standard benchmark instances and complex real-world scenarios, with detailed analysis of performance characteristics.

**Impact and Applications:**

The research has significant implications for both the theoretical understanding of location problems and their practical applications:

1. **Modeling Flexibility**: The constraint programming approach enables practitioners to easily incorporate domain-specific requirements that are challenging to express in traditional mathematical programming formulations.

2. **Solution Quality**: For complex instances with multiple interacting constraints, the approach often finds better solutions than traditional methods, particularly when optimality guarantees are not required.

3. **Practical Applications**: The improved modeling capabilities enable more realistic representation of real-world location problems in domains such as:
   - Healthcare facility planning with multi-level service requirements
   - Disaster response with backup coverage considerations
   - Retail network design with cannibalization effects
   - Telecommunications infrastructure with technology compatibility constraints

This publication represents a significant advancement in the application of constraint programming techniques to location problems, providing both theoretical insights and practical tools for solving complex real-world instances.

## Contact

- **Email**: [heythem.sattoutah@etu.sorbonne-universite.fr](mailto:heythem.sattoutah@etu.sorbonne-universite.fr)
- **LinkedIn**: [linkedin.com/in/haithem-satoutah](https://www.linkedin.com/in/haithem-satoutah/)
- **GitHub**: [github.com/satoutahhaithem](https://github.com/satoutahhaithem)
- **ORCID**: [orcid.org/0009-0004-0258-3446](https://orcid.org/0009-0004-0258-3446)

---

*This README was last updated on May 30, 2025*
