# Oil & Gas - Industrial Equipment Monitoring API

Real-time monitoring API for oil & gas equipment with anomaly detection and automatic alerts. Adapted for Sonangol / TotalEnergies / Azule Energy operations.

**Tech Stack:** Java 17, Spring Boot, REST API, MySQL, Industrial IoT Logic

**Use Case:**
This API monitors sensors (pressure, temperature, fuel level) in oil facilities. Similar to bank anti-fraud, but for industrial safety.

**Architecture:**
IoT Sensors -> API Gateway -> Monitoring Service -> Industrial DB
                         -> Anomaly Detection Service (Anti-Fraud logic adapted)
                         -> Alert System

**Key Features:**
- Real-time sensor validation before storing in Core DB
- Anomaly detection: pressure > threshold, fuel leak suspicion
- POST /api/sensors/data - receive sensor data
- GET /api/alerts - critical alerts for operations team
- Designed to reduce false alarms and save DB resources

**Industrial Value:**
Prevents equipment failure and safety risks by validating data early - same pattern used in banking Core to save Oracle costs, now applied to Oil & Gas.

**Author:** Almerindo Jamba
BSc Computer Engineering - UCAN - 4th Year
Luanda, Angola | +244 940 147 778
Focus: Backend for Industrial Systems

#oilandgas #sonangol #totalenergies #java #angola