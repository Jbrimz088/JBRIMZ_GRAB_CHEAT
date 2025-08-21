Both the injector executable and the Inno Setup installer (wizard) may be flagged by antivirus scanners (including VirusTotal).

This is a false positive — here’s why it happens:

Why the Injector Is Flagged

The program performs DLL injection, which is the same technique used by malware.
Antivirus heuristics detect any injector as potentially malicious, regardless of its purpose.
The binary is unsigned, so Windows/AV engines treat it as untrusted.

Why the Installer Is Flagged

The installer simply packages the injector, so the detection carries over.
Inno Setup executables with LZMA solid compression and uncommon names often trip heuristics.
Being a new file with no reputation, SmartScreen and AV products err on the side of caution.

Important Notes

The code is not a RAT, trojan, or virus.
The detections are heuristics-based (behavioral), not because of actual malicious payloads.
