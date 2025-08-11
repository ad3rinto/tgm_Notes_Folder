### Finance Transformation - Worldpay file tactical solution



#### Proposed Tactical Fix:



While the long-term solution will take a few sprints, we can resolve the daily disruption in under a week with a simple automated file move. I propose we implement this tactical fix immediately, while simultaneously advancing the Logic App design. This way, Finance gets relief tomorrow, and we stay on track for a robust, scalable solution down the line.





Automate file handoff via a lightweight script or scheduled task:

A simple PowerShell or Python script that:

* Monitors the inbox folder.
* Copies and renames the file as needed.
* Places it into the AutoRek intake folder automatically.
* Run via a scheduled task on a reliable server or VM (even a low-risk, existing one).

Estimated effort: 1–2 days (dev + test + deployment).



#### Why this works:



* Low complexity, high impact.
* Uses existing infrastructure (no new platform dependencies).
* Can be implemented in under a week.
* Mitigates the daily business disruption immediately.





#### Monitor \& Feedback Loop

Implement basic logging/alerting on the tactical script (e.g., “File moved at 5:05 AM”).

