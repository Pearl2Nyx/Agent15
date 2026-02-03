# Pixodex – AI Public Transport Crowd Prediction System
## Requirements Document

---

## 1. Project Overview

Pixodex is an AI-powered crowd prediction system designed to forecast bus occupancy levels in Indian metropolitan cities. The system leverages machine learning algorithms to analyze historical ridership patterns, real-time data feeds, and contextual factors to provide accurate crowd density predictions for public transport users and transit authorities.

## 2. Problem Statement

Public transport users in Indian cities face significant challenges with overcrowded buses, leading to:
- Uncomfortable and unsafe travel experiences
- Unpredictable commute times and missed connections
- Inefficient resource allocation by transport authorities
- Lack of real-time information for informed travel decisions

Current solutions provide limited or no crowd prediction capabilities, forcing commuters to rely on guesswork when planning their journeys.

## 3. Goals and Objectives

### Primary Goals
- Predict bus crowd density with 80%+ accuracy for 1-4 hour forecasts
- Reduce average passenger wait times by 15-20%
- Improve overall passenger satisfaction and safety

### Secondary Goals
- Enable data-driven bus fleet optimization for transport authorities
- Provide alternative route suggestions during peak congestion
- Create a scalable foundation for expansion to other transport modes

## 4. Target Users

### Primary Users
- **Daily Commuters**: Office workers, students, and regular public transport users
- **Occasional Travelers**: Tourists, visitors, and infrequent bus users

### Secondary Users
- **Transport Authorities**: City bus operators and fleet managers
- **Urban Planners**: Government officials responsible for transport infrastructure

## 5. Functional Requirements

### 5.1 Core Prediction Features
- **FR-001**: System shall predict crowd density levels (Low/Medium/High) for specific bus routes
- **FR-002**: System shall provide predictions for 1, 2, and 4-hour time horizons
- **FR-003**: System shall update predictions every 15 minutes during operational hours
- **FR-004**: System shall cover major bus routes in at least 2 Indian metropolitan cities

### 5.2 User Interface
- **FR-005**: Mobile-responsive web application for crowd predictions
- **FR-006**: Route search functionality with crowd level indicators
- **FR-007**: Alternative route suggestions when high crowd levels predicted
- **FR-008**: Historical crowd pattern visualization for popular routes

### 5.3 Data Integration
- **FR-009**: Integration with public transport schedule APIs
- **FR-010**: Weather data integration for improved prediction accuracy
- **FR-011**: Holiday and event calendar integration
- **FR-012**: Real-time traffic data incorporation

### 5.4 Administrative Features
- **FR-013**: Dashboard for transport authorities showing fleet utilization
- **FR-014**: Prediction accuracy monitoring and reporting
- **FR-015**: Route performance analytics and recommendations

## 6. Non-Functional Requirements

### 6.1 Performance
- **NFR-001**: System response time < 3 seconds for prediction queries
- **NFR-002**: Support for 10,000+ concurrent users during peak hours
- **NFR-003**: 99.5% system uptime during operational hours (6 AM - 11 PM)

### 6.2 Scalability
- **NFR-004**: Architecture shall support addition of new cities without system redesign
- **NFR-005**: Database shall handle 1M+ prediction requests per day

### 6.3 Accuracy
- **NFR-006**: Prediction accuracy ≥ 80% for 1-hour forecasts
- **NFR-007**: Prediction accuracy ≥ 70% for 4-hour forecasts

### 6.4 Security & Privacy
- **NFR-008**: User location data shall be anonymized and aggregated
- **NFR-009**: HTTPS encryption for all data transmission
- **NFR-010**: Compliance with Indian data protection regulations

## 7. Data Requirements

### 7.1 Historical Data
- Bus ridership patterns (6-12 months of historical data)
- Route schedules and frequency information
- Weather data (temperature, rainfall, humidity)
- Public holidays and local events calendar

### 7.2 Real-time Data Sources
- GPS tracking data from buses (simulated for prototype)
- Weather API feeds
- Traffic congestion data
- Special events and disruptions

### 7.3 External Data Integration
- Google Maps API for route information
- OpenWeatherMap API for weather data
- Public transport authority APIs (where available)
- Social media feeds for event detection (optional)

## 8. Assumptions and Constraints

### 8.1 Assumptions
- Historical ridership data can be simulated or obtained from transport authorities
- Weather significantly impacts ridership patterns
- Peak hours follow consistent patterns (7-10 AM, 5-8 PM)
- Users have smartphone access with internet connectivity

### 8.2 Constraints
- **Technical**: Limited access to real-time bus occupancy sensors
- **Data**: Dependency on third-party APIs for weather and traffic data
- **Budget**: Prototype development with limited cloud infrastructure budget
- **Timeline**: 6-month development timeline for MVP
- **Regulatory**: Compliance with local data privacy laws

### 8.3 Prototype Limitations
- Initial deployment limited to 2-3 major bus routes per city
- Simulated occupancy data for training ML models
- Basic mobile web interface (no native mobile app)

## 9. Success Metrics

### 9.1 Technical Metrics
- **Prediction Accuracy**: ≥ 80% for 1-hour forecasts, ≥ 70% for 4-hour forecasts
- **System Performance**: < 3 second response time, 99.5% uptime
- **Data Quality**: < 5% missing data points in prediction models

### 9.2 User Adoption Metrics
- **User Engagement**: 1,000+ active users within 3 months of launch
- **Usage Frequency**: Average 3+ predictions per user per week
- **User Satisfaction**: ≥ 4.0/5.0 rating in user feedback surveys

### 9.3 Business Impact Metrics
- **Operational Efficiency**: 10% improvement in bus utilization rates
- **User Experience**: 15% reduction in reported overcrowding incidents
- **Cost Savings**: Measurable reduction in operational costs for transport authorities

### 9.4 Prototype Success Criteria
- Successful deployment on 2 major routes in 1 Indian city
- Demonstration of core prediction functionality
- Positive feedback from 100+ beta users
- Technical architecture validated for future scaling

---

**Document Version**: 1.0  
**Last Updated**: February 2026  
**Next Review**: March 2026