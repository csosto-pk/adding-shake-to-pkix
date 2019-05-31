Version 00 

This document lists the external cryptographical libraries which has been vetted and approved for general use. It also lists the external libraries with approved certificate handling implementation that have been vetted and approved for general use. 

The approved versions of each listed library are all the supported versions of the specific library, unless explicitly stated in the listed library table. For example OpenSSL version 1.0.2 is scheduled to EoL 2019; hence applications need to migrate to an OpenSSL version that will receive security fixes by the end of 2019. 

To find changes since the previous version of these lists refer to the Change Log. 

Note: If a library doesn't appear on the list that you think should be included, then email ask-src-crypto@cisco.com. We won't review libraries unless people ask for them. 


Approved Crypto Libraries 
--------------------
* OpenSSL by OpenSSL 
* GoLang by Google - Not FIPS approved. Check SpeceMonkey for FIPS.  
* SpaceMonkey - This is not actually a library; instead it is a shim layer that connects Go routines to a CiscoSSL/OpenSSL compatible library for FIPS. This underlying library must be approved as well. 


Approved Certificate Handling Libraries 
--------------------
* OpenSSL - Note: Version 1.0.2 is scheduled to EoL 2019; hence applications need to migrate to an OpenSSL version that will receive security fixes


Change Log
--------------------

* v00 5/29/2019
  First initial version of the approved libraries
