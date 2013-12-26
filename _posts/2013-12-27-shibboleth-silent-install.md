---
layout: post
title:  "How to do a silent install for Shibboleth"
date:   2013-12-27 10:00:00
categories: personal blog shibboleth deployment
---

When trying to a silent install with shibboleth you may find that it freezes and never finishes.  The reason for this is caused by the WiX installer UI
initializing some variables and with the silent install the UI doesn't open to initialize the variables.  This can be solved easily be passing the
variables as command line arguements.  Below is the command line arguements to accomplish silent install (The ISAPI filters may still need to be installed manually).

``msiexec /qn /i shibboleth-sp-2.5.1-win64.msi REBOOT=ReallySupress INSTALL_ISAPI_FILTER=FALSE INSTALL_32BIT=FALSE SHIB_FILE_EXTENSION=shb INSTALLDIR=C:\shibstuff5\``