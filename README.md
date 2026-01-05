
# 🏥 AI-Based Securty for Healthcare Applications
This project focuses on securing sensitive healthcare data using AI-driven adaptive encryption techniques. It addresses the challenge of balancing strong security with system performance in dynamic and resource-constrained healthcare environments such as IoT devices, cloud-based EHR systems, and real-time patient monitoring platforms.

The system integrates cryptographic algorithms (AES, ECC, RSA) with machine learning–based decision-making and anomaly detection to dynamically select optimal encryption strategies based on real-time system conditions.

## Problem Statement

Healthcare systems face increasing security risks due to:

Transmission of sensitive data over unstable or low-resource networks

High computational overhead of traditional encryption methods

Inflexible static encryption schemes

Increased cyberattacks on IoT-enabled healthcare systems

This project proposes an AI-powered adaptive encryption framework that ensures robust security while maintaining efficiency and responsiveness.

## Objectives

Protect patient records and healthcare communications using AI-driven encryption

Ensure secure data storage and transmission across heterogeneous networks

Detect anomalies and suspicious activities using intelligent monitoring

Dynamically adapt encryption algorithms and key strengths in real time

Enable secure and tamper-proof cryptographic key exchange

## System Architecture
User Roles and Access Control

Doctor: Manage patients, upload prescriptions, request and view lab reports

Patient: Book appointments, view diagnoses and lab results

Lab Technician: Upload lab test results

Authentication and authorization ensure role-based dashboard access.

## Secure Data Flow

All sensitive data is encrypted before database storage

Only authorized users can decrypt and access information

Digital signatures verify data integrity and authenticity

## Core Technologies and Algorithms
**AES (Advanced Encryption Standard)**

Symmetric encryption for securing data at rest

Encrypts patient records, prescriptions, diagnoses, and lab reports

Ensures confidentiality and regulatory compliance

**ECC(Elliptic Curve Cryptography)**

Used for secure AES key exchange

Enables digital signatures for integrity verification

Lightweight and suitable for IoT and mobile healthcare devices

**RSA (Rivest–Shamir–Adleman)**

Asymmetric encryption for secure key exchange and signatures

Provides authentication and non-repudiation

## AI-Powered Adaptive Encryption

Uses a Random Forest machine learning model to dynamically select encryption strategies

Evaluates real-time parameters including:

CPU usage

File size

User role

Network latency and traffic

Anomaly score

Supported Encryption Modes

AES-128, AES-192, AES-256

Hybrid ECC + AES

RSA-based encryption

Encryption strength automatically increases during high-risk or abnormal conditions.

## Anomaly Detection System

A hybrid AI-based detection framework using:

Isolation Forest

One-Class SVM

Random Forest

Autoencoder

Detection Capabilities

Suspicious login attempts

Abnormal encryption parameters

Unusual CPU or network usage

Invalid key lengths or tampered uploads

Automated Responses

Key rotation

Stronger encryption enforcement

Session blocking

## Applications

Secure Remote Patient Monitoring systems

Protection of smart medical implants such as pacemakers and insulin pumps

Secure cloud-based Electronic Health Records

Emergency data transmission from smart ambulances

Home healthcare IoT device security

Smart hospital infrastructure protection

## Outcomes

Improved confidentiality, integrity, and availability of healthcare data

Reduced computational overhead through adaptive encryption

Real-time detection and mitigation of security threats

Scalable and modular security architecture for future healthcare systems

### 💻 Frontend Experience
- **Responsive Design**: Built with Bootstrap for a clean, mobile-friendly UI.
- **Role-based Dashboards**: Unique interfaces for each user type (Doctor, Patient, Lab).
- **Real-time Updates**: Smooth navigation and form feedback for improved UX.

## 🧰 Tech Stack

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| Django          | Backend web framework            |
| SQLite          | Lightweight database             |
| Bootstrap       | Frontend styling                 |
| HTML/CSS        | Page structure and design        |
| JavaScript      | Basic interactivity              |

## Screenshots
<img width="772" height="641" alt="Screenshot 2025-05-26 200838" src="https://github.com/user-attachments/assets/9a989959-4a39-4c73-9252-67d20d747b5a" />
<img width="1627" height="892" alt="Screenshot 2025-05-26 200405" src="https://github.com/user-attachments/assets/ff2e78a0-325f-4766-a2ca-aca677c76c3c" />
<img width="1688" height="636" alt="Screenshot 2025-05-26 200453" src="https://github.com/user-attachments/assets/2067c015-d48c-4688-8dc0-d2ce2a4bb80e" />
<img width="765" height="846" alt="Screenshot 2025-05-26 200524" src="https://github.com/user-attachments/assets/6c90dd22-181d-4c8b-9514-62fe6934b3fe" />
<img width="909" height="380" alt="Screenshot 2025-05-26 200635" src="https://github.com/user-attachments/assets/bc733cac-32fb-4256-a077-8590d1b0fca9" />
<img width="1863" height="813" alt="Screenshot 2025-05-26 200646" src="https://github.com/user-attachments/assets/7aa40dce-e725-4f65-b094-9d4c969df596" />
<img width="1905" height="880" alt="Screenshot 2025-05-26 200721" src="https://github.com/user-attachments/assets/c767bb16-f41d-4055-9b8c-a7f34c153bfe" />
<img width="1911" height="734" alt="Screenshot 2025-05-26 200743" src="https://github.com/user-attachments/assets/3ea8684f-6192-422a-8a77-6fc7e51ad80c" />
<img width="1910" height="737" alt="Screenshot 2025-05-26 200756" src="https://github.com/user-attachments/assets/6c1f5b57-4bc5-45ef-bce4-6b192c89d206" />


## Conclusion

This project demonstrates a secure-by-design healthcare security framework that combines cryptography and artificial intelligence. By integrating AES for data security, ECC and RSA for key management and digital signatures, and machine learning–based adaptive decision-making, the system ensures robust protection of sensitive healthcare data without compromising performance.

The solution is suitable for real-world deployment in IoT-enabled healthcare ecosystems, smart hospitals, and cloud-based medical platforms.




## 🔧 Setup

```bash
git clone https://github.com/yourusername/healthcare.git
cd healthcare
python -m venv venv
source venv/bin/activate  # On Windows: venv\\Scripts\\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
