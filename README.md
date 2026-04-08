<img width="931" height="624" alt="imag " src="https://github.com/user-attachments/assets/35afa8da-b511-402e-9cc0-370954557631" />

🧠 Core Design Overview

We model the system around these main entities:

Patient
Doctor
Department (Specialty)
Appointment (Visit)
Consultation
Prescription/Test Order
Diagnostic Test
Test Report
Payment
🔗 Relationships Explained Clearly
1. Patient ↔ Appointment
One patient → many appointments
Each appointment → one patient

👉 Patient (1) —— (M) Appointment

2. Doctor ↔ Appointment
One doctor → many appointments

👉 Doctor (1) —— (M) Appointment

Appointment ↔ Consultation
Each appointment has one consultation

👉 Appointment (1) —— (1) Consultation

5. Consultation ↔ Prescription/Test Order
One consultation → multiple Prescription/Test Order

👉 Consultation (1) —— (M) Prescription/Test Order
