# Linux Architecture Reference Specification for OpenPOWER
This repository hold the source for the source for the
Linux on Power Architecture Reference documents.  There are
multiple component documents as follows:

* The Platform (../Platform/) document describes the basic
requirements to run Linux on the hardware platform.

* The Device Tree (../DeviceTree/) document describes the
structure and bindings associated with the device tree 
definitions for OpenPOWER systems.

* The Error Handing (../ErrorHandling/) document describes
the error reporting and recommended error procedures for the system.

* The run-time services or RTAS (../RTAS/) document describes
the firmware interfaces available to Linux running on the system
and in a VM.

* The Virtualization (../Virtualization/) document describes the
environment by which virtualized OS images are run on the system.

The basis for this document was the
[*Linux on Power Architecture Platform Reference (LoPAR)*](https://openpowerfoundation.org/?resource_lib=linux-on-power-architecture-platform-reference) 
Version 1.1, March 2016.  It was derived from an IBM document known as the *Power Architecture Platform Reference (PAPR)* Versions 2.7.  While much of this
documentation may apply to the IBM PowerVM (LPAR) environment, it will serve as a good base for the OpenPOWER documentation effort as well as support the
more broad IBM Linux on Power community as well.

To build this project, one must ensure that the Docs-Master project has
also been cloned at the same directory level as the Docs-Template project.
This can be accomplished with the following steps:

1. Clone the master documentation project (Docs-Master) using the following command:

  ```
  $ git clone https://github.com/OpenPOWERFoundation/Docs-Master.git
  ```
  
2. Clone this project (Docs-Template) using the following command:

  ```
  $ git clone https://github.com/OpenPOWERFoundation/Linux-Architecture-Reference.git
  ```
  
3. Build the project with these commands:
  ```
  $ cd Linux-Architecture-Reference
  $ mvn clean generate-sources
  ```

The online version of the document can be found in the OpenPOWER Foundation
Document library at [TBD](http://openpowerfoundation.org/?resource_lib=tbd)


## Contributions
To contribute to the OpenPOWER Foundation template document project, contact Jeff Scheel \([scheel@us.ibm.com](mailto://scheel@us.ibm.com)\) or 
Jeff Brown \([jeffdb@us.ibm.com](mailto://jeffdb@us.ibm.com)\).

Contributions to this project should conform to the `Developer Certificate
of Origin` as defined at http://elinux.org/Developer_Certificate_Of_Origin.
Commits to this project need to contain the following line to indicate
the submitter accepts the DCO:
```
Signed-off-by: Your Name <your_email@domain.com>
```
By contributing in this way, you agree to the terms as follows:
```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
660 York Street, Suite 102,
San Francisco, CA 94110 USA

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.


Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

