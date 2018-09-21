                                                      QNX

QNX is a mobile operating system that was originally developed for embedded systems and in the early 1980s by Canadian company Quantum Software Systems, later renamed QNX Software Systems and ultimately acquired by BlackBerry in 2010. The operating system’s developer, QNX Software Systems, was acquired by Research in Motion (RIM) and the OS adapted for use in the BlackBerry Playbook tablet. The version of QNX used in the Playbook is known as the QNX Neutrino real-time operating system (RTOS).

Description

The Unix-like QNX OS is microkernel-based, which means that it is a small program and elements of the operating system run as tasks that the developer can turn off if they aren’t required in a particular system. This contrasts with the traditional monolithic OS architecture, in which the operating system runs as a single program.

Interesting details:

QNX competes in the tablet market with Apple’s iOS and Google’s Android operating systems. The operating system is also expected to replace the BlackBerry OS used in the company’s smartphones.

Technology

The QNX kernel (procnto) contains only CPU scheduling, interprocess communication, interrupt redirection and timers. Everything else runs as a user process.

QNX interprocess communication consists of sending a message from one process to another and waiting for a reply. This is a single operation, called MsgSend. The message is copied, by the kernel from the address space of the sending process to that of the receiving process. If the receiving process is waiting for the message, control of the CPU is transferred at the same time, without a pass through the CPU scheduler.

 Thus, sending a message to another process and waiting for a reply does not result in "losing one's turn" for the CPU. This tight integration between message passing and CPU scheduling is one of the key mechanisms that makes QNX message passing broadly usable.
