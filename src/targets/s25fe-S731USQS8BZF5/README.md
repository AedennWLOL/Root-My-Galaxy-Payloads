# s25fe-S731USQS8BZF5

```text
device: Samsung Galaxy S25 FE (SM-S731U, s25fe)
firmware: S731USQS8BZF5 / AT&T
display build: BP3A.260607.001.S731USQS8BZF5
fingerprint: samsung/s25fexxx/s25fe:16/BP3A.260607.001/S731USQS8BZF5:user/release-keys
kernel: 6.1.157-android14-11
raw kernel SHA-256: 06026A598A04810A5EAC49511442798AFBC5F4EF926BB5191C165A484F4BB035
```

`target.h` contains the exact symbol, layout, physical-load, trace, and KASLR
values recovered from that firmware. `p0_fingerprint.h` contains 32 target
kernel page fingerprints and was checked against all 256 source qwords.

Physical load offset was verified from the sboot kernel-entry sequence
(adrp/ldr/mov w9,#-0x80000000/add/blr at sboot file offset 0x34bf4) matching
PORTING.md section 4, giving P0_PHYS_OFFSET = P0_KERNEL_PHYS_LOAD =
0x80000000 (text_offset == 0).

The profile and build artifacts are statically verified but hardware-untested.
