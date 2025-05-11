# Requirement Analysis in Software Development.
This repository is dedicated to exploring the critical phase of **Requirement Analysis** in the software development lifecycle33.

## What is Requirement Analysis?
Requirement Analysis is a critical phase in the software development lifecycle (SDLC) where the project team gathers, analyzes, and defines the requirements of the software product to be developed. This process ensures that all stakeholders have a clear and mutual understanding of what the system should do and how it should perform.

## Key Activities in Requirement Analysis.
- Requirement Gathering
  - Engage with stakeholders to collect initial requirements.
  - Use various techniques like interviews, surveys, and workshops
- Requirement Elicitation
  - Refine and elaborate on the gathered requirements.
  - Use techniques like brainstorming, focus groups, and prototyping.
- Requirement Documentation
  - Document the requirements in a detailed and structured format.
  - Use requirement specification documents, user stories, and use cases.
- Requirement Analysis and Modeling
  - Analyze and prioritize the requirements.
  - Create models to visualize and understand the requirements.
- Requirement Validation
  - Review and validate the requirements with stakeholders.
  - Define acceptance criteria and ensure traceability.

## Types of Requirements.
### Functional Requirements.
Describe what the system should.
Detailed analysis on functional requirements baaed on this [articles](https://medium.com/nerd-for-tech/system-design-architecture-for-hotel-booking-apps-like-airbnb-oyo-6efb4f4dddd7) give us the following functional requirements;

#### Hotel Management Service
- Hotel managers can:
  - Access a dedicated portal.
  - Add, update, or delete hotel listings.
  - Manage pricing, availability, and amenities.
  - View bookings for their hotels.
    
#### View Booking Service
- Users (managers and customers) can:
  - View past and current bookings.
  - Access recent data via Redis.
  - Retrieve archived data from Cassandra.

#### Notifications & Analytics
- System must:
  - Send real-time notifications for bookings and promotions.
  - Use Apache Streaming to store events in Hadoop.
  - Support data analysis for insights and customer segmentation.

#### Customer Service (Search + Booking)
- Customers can:
  - Register and log in.
  - Search for hotels using filters (location, rating, price).
  - View detailed hotel information, offers, and recommendations.
  - Book hotels and receive confirmation.
  - Make payments via integrated third-party services.
  - Receive booking and promotional notifications.

- System functions:
  - Search via Elasticsearch.
  - Cache frequent data in Redis.
  - Queue updates using Kafka or RabbitMQ.
  - Archive data in Cassandra for long-term storage.
  ---

### Non-functional Requirements.
Describe how the system should perform.

Detailed analysis on functional requirements baaed on this [articles](https://medium.com/nerd-for-tech/system-design-architecture-for-hotel-booking-apps-like-airbnb-oyo-6efb4f4dddd7) give us the following non functional requirements;
#### Scalability
- Handle high user traffic with microservice architecture.
- Use distributed systems (Kafka, Cassandra, Redis) for scaling.
#### Performance
- Optimize API response time using:
  - Load balancers.
  - Redis caching.
  - CDN delivery.
#### Reliability and Availability
- Ensure uptime with:
  - Master-slave DB replication.
  - Server clustering and failover handling.
#### Security
- Secure user data and authentication.
- Use encrypted payment gateways.
#### Maintainability & Modularity
- Microservices allow independent development and scaling.
- Services are decoupled and maintainable.
#### Data Analytics
- Store logs and events in Hadoop for business insights.
- Analyze booking patterns and customer behaviors.
#### Real-time Processing
- Deliver instant notifications using Kafka consumers.
- Process and display updates without delay.

## Why is Requirement Analysis Important?”
- Clarity and Understanding: It helps in understanding what the stakeholders expect from the software, reducing ambiguity.
- Scope Definition: Clearly defines the scope of the project, which helps in preventing scope creep.
- Basis for Design and Development: Provides a solid foundation for designing and developing the system.
- Cost and Time Estimation: Facilitates accurate estimation of project cost, resources, and time.
- Quality Assurance: Ensures that the final product meets the specified requirements, leading to higher customer satisfaction.



