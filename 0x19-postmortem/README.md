Postmortem Summary: Ubuntu Container's Nginx Port 80 Listening Issue
Incident Summary:
On November 12, 2023, at approximately 14:00, our Ubuntu container hosting Nginx faced an unexpected issue, preventing it from listening on port 80. This resulted in a service disruption for users attempting to access web content served by Nginx. This postmortem aims to analyse the incident, identify the root cause, outline resolution steps, and establish preventive measures.
Incident Timeline:
12/11/2023-14:00: Initial reports indicated users couldn't access web content on Nginx via port 80.
13/11/2023-09:00: Monitoring detected no response on port 80, triggering alerts.
13/11/2023-12:00: Incident response team initiated an investigation.
14/11/2023-08:00: Confirmed Nginx wasn't listening on port 80, causing service disruption.
14/11/2023-10:00: System admins and DevOps engineers collaborated to troubleshoot.
14/11/2023-16:00: Issue resolved; Nginx resumed normal operation on port 80.
18/11/2023-11:00: Post-incident analysis began to understand factors causing Nginx port 80 unavailability.
Root Cause Analysis:
The root cause of the Nginx port 80 listening issue was [provide detailed explanation of the root cause]. Possible causes could include misconfigurations, conflicting processes, or network-related issues. In this case, [explain how the root cause led to Nginx not listening on port 80].
Corrective Resolution:
To address the issue, the following steps were taken:
Immediate Mitigation: Implemented a temporary workaround redirecting traffic to an alternate port (e.g., 8080) to minimise user impact.
Configuration Review: Thoroughly reviewed Nginx configuration files to identify misconfigurations or discrepancies.
Process Termination: Identified and terminated conflicting processes that might have prevented Nginx from binding to port 80.
Port Availability Check: Ensured port 80 was available and not occupied by other services.
Nginx Restart: Gracefully restarted Nginx to apply necessary configuration changes.
Preventive Measures:
To prevent similar incidents, the following measures have been implemented:
Automated Configuration Checks: Implemented automated checks to validate Nginx configuration file correctness during deployments.
Monitoring and Alerts: Enhanced monitoring to promptly detect anomalies in Nginx behaviour, with specific alerts for port availability.
Documentation Update: Ensured documentation is up-to-date, including guidelines for troubleshooting and resolving Nginx port-related issues.
Regular Audits: Scheduled regular audits of the web stack to identify and rectify potential misconfigurations or conflicts.
Conclusion:
This postmortem offers a detailed analysis of the Nginx port 80 listening issue, encompassing the incident timeline, root cause analysis, resolution steps, and preventive measures. We appreciate your understanding and apologise for any inconvenience caused. Our team remains dedicated to maintaining a reliable web stack, continuously improving to prevent similar incidents in the future.
Please feel free to reach out if you have any further questions or concerns.
Sincerely,
ALX Cohort 14
Theresa Abutu

