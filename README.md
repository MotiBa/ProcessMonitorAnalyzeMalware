# ProcessMonitorAnalyzeMalware
Script to parse Process Monitor XML log file, and give you a summary report.
The report conaints sections dedicated to Processes Created, File Activity, Registry Activity, Network Traffic, and Unique Hosts

Instructions to prepare the Process Monitor trace this script requires:
   Start Procmon. 
   Stop the Procmon trace.
   Add an Include filter for "Result is SUCCESS".
    Save the trace:
    * Events displayed using current filter
    * DO NOT SELECT Also include profiling events
    * Format XML - do not check the stack traces or stack symbols options

EXAMPLE:
   .\Analyze-ProcmonLog.ps1 .\Logfile.XML 
