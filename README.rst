nosnap-deb
==========

Provides a dummy ``ubuntu-system-adjustments`` package so *Linux Mint
firefox* will install on *Ubuntu* (or *Debian*).

Places ``nosnap.pref`` in ``/etc/apt/preferences.d/``.

See: `<https://wjd.nu/notes/2022#ubuntu-snap-mint-chromium>`_


Building / installing
---------------------

::

    dpkg-buildpackage -us -uc
    dpkg -i ../nosnap_0.1_all.deb
    apt-get install firefox
