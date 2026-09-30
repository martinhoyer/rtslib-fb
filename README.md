rtslib
======

A Python object API for managing the Linux LIO kernel target
------------------------------------------------------------
rtslib is an object-based Python library for configuring the LIO
generic SCSI target, present in Linux kernel.


rtslib development
------------------
rtslib is licensed under the Apache 2.0 license. Contributions are welcome.

 * Source repo: [GitHub](https://github.com/open-iscsi/rtslib-fb)
 * Bugs: [GitHub](https://github.com/open-iscsi/rtslib-fb/issues)
 * Releases: [PyPI](https://pypi.org/project/rtslib/)

Packages
--------
rtslib is packaged for a number of Linux distributions including
RHEL,
[Fedora](https://src.fedoraproject.org/rpms/python-rtslib),
openSUSE, Arch Linux,
[Gentoo](https://packages.gentoo.org/packages/dev-python/rtslib-fb), and
[Debian](https://tracker.debian.org/pkg/python-rtslib-fb).

Contribute
----------
rtslib complies with PEP 621 and as such can be built and installed with tools like `build` and `pip`.

For development, consider using [Hatch](https://hatch.pypa.io):  
`hatch shell` to create and enter a Python virtualenv with the project installed in editable mode  
`pre-commit install` to enable pre-commit hooks  
`hatch build` to create tarball and wheel  

Formerly rtslib-fb
------------------
This project was previously published as `rtslib-fb` ("free branch"), a fork
of the original "rtslib" code written by RisingTide Systems. The fork has long
been the only maintained version, so the `-fb` suffix has been dropped and
releases are now published on PyPI as `rtslib`.

The `rtslib_fb` module is kept as a deprecated alias of `rtslib`, so existing
`import rtslib_fb` code keeps working. New code should `import rtslib`.

If you are upgrading an existing pip installation, uninstall the old
distribution first, since both install the same files:

    pip uninstall rtslib-fb
    pip install rtslib
