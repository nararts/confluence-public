# Playback and crash diagnostics

In Confluence 2.4.77 for Windows, open Settings > Diagnostics and select Check application. The checks report engine components and startup, test WAV decoding, a public catalogue response, recent error categories and available crash logs.

Select Copy report to share the results. Review the report before publishing it. Do not share passwords, access tokens or account sessions.

The local crash log is stored under `%LOCALAPPDATA%\Confluence\Logs\crash.log`. A previous bounded log may also exist. Forced process termination or native runtime failures may not leave a managed crash log.

A successful WAV decode does not verify that speakers are audible. A successful catalogue check does not prove every service or track is available. Historical crash records do not automatically identify the cause of the current problem.

If Windows prevents the app from opening, an in-app check cannot run. The blocked file and process may be identified in Windows Event Viewer under CodeIntegrity > Operational or in an Application Error event. A security warning alone is not proof of malware, and a clean scan is not an absolute guarantee of safety.
