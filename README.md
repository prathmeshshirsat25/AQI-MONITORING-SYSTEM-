# Precision AQI Monitoring and Prediction System

## Project Overview

Precision AQI Monitoring and Prediction System is a software focused IoT solution developed for real time air quality monitoring, intelligent AQI calculation, predictive analysis, and automated alert generation. The system combines embedded programming, sensor data processing, and software based filtering techniques to improve monitoring accuracy while maintaining a low cost architecture.

The project continuously collects environmental data using multiple sensors and processes the readings through a custom built filtering pipeline to reduce noisy values and improve reliability. A major focus of the implementation was software optimization and data accuracy enhancement instead of relying solely on expensive hardware.

---

# Features

* Real time AQI monitoring
* Multi sensor data acquisition
* Smart AQI prediction and analysis
* Automated SMS alert system
* Dynamic sensor calibration
* Temperature and humidity compensation
* Multi level software based filtering
* Real time LCD monitoring interface
* Cost optimized IoT architecture

---

# Sensors and Modules Used

| Component        | Purpose                          |
| ---------------- | -------------------------------- |
| MQ 7 Sensor      | Carbon Monoxide detection        |
| MQ 135 Sensor    | VOC and air quality sensing      |
| GP2Y Dust Sensor | PM concentration monitoring      |
| DHT11            | Temperature and humidity sensing |
| GSM Module       | SMS alert notifications          |
| LCD Display      | Real time data visualization     |
| Arduino          | Embedded processing and control  |

---

# Software Architecture

## 1. Sensor Data Acquisition

The system continuously collects analog sensor readings from PM, CO, and VOC sensors while also monitoring environmental conditions such as temperature and humidity.

## 2. Dynamic Calibration System

Implemented automatic sensor calibration during startup to establish environment specific baseline resistance values for MQ sensors. This improves reliability across different deployment environments.

## 3. Multi Stage Filtering Pipeline

Designed a custom 5 layer filtering mechanism for improving data precision and reducing unstable sensor outputs.

### Filtering Techniques Used

* Rapid sample averaging
* Heavy software smoothing
* Voltage spike protection
* Environmental compensation
* Signal stabilization

This filtering architecture significantly reduced noisy readings and improved overall monitoring accuracy to approximately 94 percent.

## 4. AQI Computation Engine

Implemented AQI calculation logic using EPA based breakpoint conversions for:

* PM2.5 concentration
* Carbon Monoxide levels
* VOC concentration

The final AQI value is generated using the highest pollutant impact method.

## 5. Predictive Monitoring and Alerts

The software continuously evaluates AQI trends and automatically triggers SMS alerts whenever air quality crosses predefined safety thresholds.

## 6. Real Time Display System

Designed a dual screen LCD interface for displaying:

* AQI status
* Pollutant concentration
* Temperature and humidity
* Sensor calibration values

---

# Key Software Concepts Implemented

* Embedded C programming
* Real time sensor processing
* Data filtering algorithms
* Signal smoothing techniques
* Environmental compensation logic
* AQI computation models
* Serial communication
* GSM based notifications
* IoT monitoring workflows

---

# Performance Improvements

| Optimization               | Impact                           |
| -------------------------- | -------------------------------- |
| 10 sample averaging        | Reduced random fluctuations      |
| Heavy smoothing algorithm  | Improved reading stability       |
| Dynamic Ro calibration     | Better environmental adaptation  |
| Voltage spike protection   | Prevented invalid sensor outputs |
| Temp humidity compensation | Improved sensor consistency      |

---

# Achievements

* Reduced system cost to nearly one tenth of traditional solutions
* Achieved approximately 94 percent monitoring accuracy
* Built a custom software driven filtering pipeline
* Selected among the Top 5 Finalists in INC

---

# Future Enhancements

* Cloud based monitoring dashboard
* Machine learning based AQI prediction
* Mobile application integration
* Historical data analytics
* Wireless IoT communication
* Advanced anomaly detection

---

# Technologies Used

* Embedded C
* Arduino IDE
* IoT Concepts
* Sensor Data Processing
* GSM Communication
* AQI Computation Logic
* Software Filtering Algorithms

---

# Conclusion

This project demonstrates how intelligent software engineering and efficient data processing can significantly improve the reliability and affordability of environmental monitoring systems. By focusing on filtering algorithms, sensor optimization, and predictive monitoring, the system delivers accurate AQI insights while remaining scalable and cost effective for real world applications.
