.. include:: ../../Includes.txt


.. _updating-typo3:

Keep the TYPO3 core up-to-date
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As described in chapter :ref:`typo3-versions`, a new version
of TYPO3 can either be a major update (e.g. from version 4.x.x to
version 6.x.x), a minor update (e.g. from version 6.1.x to version
6.2.x) or a maintenance/bugfix/security release (e.g. from version
6.1.4 to 6.1.5).

In most cases, a maintenance/bugfix/security update is a no-brainer,
see :ref:`TYPO3 Installation and Upgrade Guide <t3install:start>`
for further details.

When you extract the archive file of new TYPO3 sources into the
existing install directory (e.g. the web root of your web server) and
update the symbolic links, pointing to the directory of the new version,
do not forget to **delete** the old and possibly insecure TYPO3 core
version. Failing doing this creates the risk of leaving the source code
of the previous TYPO3 version on the system and as a consequence, the
insecure code may still be accessible and a security vulnerability
possibly exploitable.

Another option is to store the extracted TYPO3 sources outside of the
web root directory (so they are not acceessible via web requests) as
a generale rule and use symblic links inside the web root to point to
the correct and secure TYPO3 version.

