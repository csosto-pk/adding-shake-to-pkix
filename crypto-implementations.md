Version 00 

This document lists the external [cryptographical libraries](#approved-crypto-libraries) which have been vetted and approved for general use. It also lists the external [libraries](#approved-certificate-handling-libraries) with approved certificate handling implementations that have been vetted and approved for general use. 

The approved versions of each listed library are all the supported versions of the specific library, unless explicitly stated in the listed library table. 

To find changes since the previous version of these lists refer to the Change Log. 

**Note**: If a library doesn't appear on the list that you think should be included, then email ask-src-crypto@cisco.com. We won't review libraries unless people ask for them. 



Approved Crypto Libraries
--------------------
* OpenSSL by OpenSSL. The approved versions are *1.1.1* and above - Version 1.0.2 is scheduled to EoL 2019; hence applications need to migrate to an OpenSSL version that will receive security fixes by the end of 2019.
* GoLang by Google - The approved versions are *1.12* and above - GoLang is not FIPS approved. Check SpeceMonkey for FIPS.  
* SpaceMonkey - This is not actually a library; instead it is a shim layer that connects Go routines to a CiscoSSL/OpenSSL compatible library for FIPS. This underlying library must be approved as well. 



Approved Certificate Handling Libraries
--------------------
* OpenSSL - The approved versions are *1.1.1* and above - Version 1.0.2 is scheduled to EoL 2019; hence applications need to migrate to an OpenSSL version that will receive security fixes



Evaluated but not Approved Libraries
--------------------
* BouncyCastle by the	Legion of the Bouncy Castle 

This library includes the Dual-EC random number generator - including that library (even if unused) is not acceptable. BouncyCastle includes cryptographical algorithms with potental IPR claims (OCB); potential legal risk. This library is also known to have poor side channel resistance; this may be a concern for some uses. Use of [CiscoJ](https://apps.na.collabserv.com/communities/service/html/communitystart?communityUuid=d15ca1a1-4805-4df7-a433-46f0d74eee2d) as an alternative is recommended



Change Log
--------------------

* v00 5/29/2019
  First initial version of the approved libraries
