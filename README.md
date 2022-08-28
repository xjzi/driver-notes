# Designing a kernel module and SATA / SAS device
I think we should do [SATA](sata.md) because I want to replace my laptop's CD drive with a custom peripheral.
SATA is implemented over the 8b/10b protocol, which is usually implemented on the [FPGA](fpga.md) level.

Aug 28, 2022.
I'm new to github, and this would be my first official readme. I've been observing SATA design structures, and here is what I came up with:

  Serial Advanced Technology Attachment (SATA) is a serial point-to-point half-duplex computer bus, and protocol.
  SATA has 4 layers; Physical, datalink, tranport, and application.
  SATA data connector has 7 pins; 4 data, 3 ground.
  SATA implements 8b/10b encoding at the data-link layer.
  SATA revisions; Rev 1.0 (1.5 GB/s), rev 2.0 (3.2 GB/s), and rev 3.0 (up to 6 GB/s).

Citation:
https://community.element14.com/technologies/embedded/b/blog/posts/storage-insights-6---guide-to-sata-serial-ata
https://faculty.cs.niu.edu/~berezin/463/lec/bus/sata.html
