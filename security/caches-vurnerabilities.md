# Caches Vurnerabilities
## Meltdown and Spectre - Professor Mark Handley, UCL
The Meltdown and Spectre vulnerabilities in almost all modern CPUs have received a great deal of publicity in the last week. Operating systems and hypervisors need significant changes to how memory management is performed, CPU firmware needs updating, compilers are being modified to avoid risky instruction sequences, and browsers are being patched to prevent scripts having access to accurate time. All this because of how speculative execution is handled in modern pipelined superscalar CPUs, and how side-channel attacks reveal information about execution that the CPU tries to pretend did not happen. Mark Handley will explain what modern CPUs actually do to go fast, discuss how this leads to the Meltdown and Spectre vulnerabilities, and summarize the mitigations that are being put in place.

[![Spectre: Secrets, Side-Channels, Sandboxes, and Security](https://lh3.googleusercontent.com/z6Sl4j9zQ88oUKNy0G3PAMiVwy8DzQLh_ygyvBXv0zVNUZ_wQPN_n7EAR2By3dhoUpX7kTpaHjRPni1MHwKpaBJbpNqdEsHZsH4q)](https://youtu.be/m66EAgRMmi8) 

## Spectre: Secrets, Side-Channels, Sandboxes, and Security
The discovery of speculative execution side-channel attacks (called "Spectre") fundamentally changes the security model of every modern superscalar microprocessor. Extracting secret data (credit cards, cryptographic keys) through side-channels is not new and has challenged the cryptographic community for decades. Despite this, the industry has often been complacent in our response, viewing these attacks as impacting a tiny amount of code and being nearly impossible to weaponize. But speculative execution attack techniques have fundamentally altered the ease and applicability of side-channels, making them a serious threat to computer security. Responding to these issues has impacted CPU design, compiler design, library design, sandbox techniques and even the C++ programming language and standard. 

[![Spectre: Secrets, Side-Channels, Sandboxes, and Security](https://lh3.googleusercontent.com/z6Sl4j9zQ88oUKNy0G3PAMiVwy8DzQLh_ygyvBXv0zVNUZ_wQPN_n7EAR2By3dhoUpX7kTpaHjRPni1MHwKpaBJbpNqdEsHZsH4q)](https://www.youtube.com/embed/_f7O3IfIR2k) 

## Spectre Explained - The Attack that took the world by surprise in 2018
Spectre is a side-channel attack that leverage speculative execution to get sensitive information stored in the CPU, intel back in 2018 struggling with this attack so much it had to disable this feature which slowed down the cpus significantly.

[![Spectre: Secrets, Side-Channels, Sandboxes, and Security](https://lh3.googleusercontent.com/z6Sl4j9zQ88oUKNy0G3PAMiVwy8DzQLh_ygyvBXv0zVNUZ_wQPN_n7EAR2By3dhoUpX7kTpaHjRPni1MHwKpaBJbpNqdEsHZsH4q)](https://youtu.be/Phmt8UrofDY) 

 
