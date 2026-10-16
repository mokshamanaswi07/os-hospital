# Hospital OS

Real-time patient monitoring for a hospital ward. Hospital OS shows live vital signs, grades each patient by triage level, assigns beds, equipment and staff automatically, and flags unreliable sensor readings.
 
Built as the Operating Systems course project *Adaptive Medical Trust Device Scheduling Framework for Intelligent Resource Allocation in Critical Care Systems* at Vellore Institute of Technology.

## Features

- **Live Monitor:** vital signs for every monitored patient, updated every 3 seconds, with an activity and alert log.
- **Patients:** admit and discharge patients, attach or remove sensors, start or stop monitoring.
- **Sensors:** live multi-sensor chart with the safe range, per-sensor cards with trend, battery and reliability score.
- **Automatic triage:** each patient is graded Stable, Serious or Critical from their combined readings.
- **Sensor reliability:** every sensor gets a 0–100% score. Low-reliability readings can't escalate a patient to Critical and are logged as low-confidence instead of raising an alarm.
- **Resources:** ICU beds, ventilators, blood units, staff and more are assigned and released automatically as triage changes, with a capacity overview, waiting list and continuous safety check.
- **Shift report:** one-click CSV export of patients, sensors, resources and events.
- **Database:** everything is stored in a local SQLite database (`hospital.db`).

https://hospital-os-web.vercel.app
