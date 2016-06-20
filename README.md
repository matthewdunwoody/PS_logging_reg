# PS_logging.reg

A Windows REG file to enable all default PowerShell logging on a system with PowerShell v5 installed. This file will modify the registry to enable:
  - Module logging for all modules
  - Script block logging
  - Transcription with:
    - Default directory selected (user's documents folder)
    - Invocation header enabled

# Usage

Import using regedit - either through the UI (file -> import) or command line (regedit.exe PS_logging.reg)

To change the output directory for transcripts, set the value for: "HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Policies\Microsoft\Windows\PowerShell\Transcription\" -> "OutputDirectory"=""

# References

https://www.fireeye.com/blog/threat-research/2016/02/greater_visibilityt.html
