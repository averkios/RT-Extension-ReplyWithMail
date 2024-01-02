### NAME
    RT-Extension-ReplyWithMail - Reply to the ticker using your default mail client

### DESCRIPTION
This extension adds an extra action in your actions menu, named "ReplyWithMail". This action uses the mailto: HTML tag to generate a base mail structure, so that you can reply using your native email client instead of RT's WebUI

### RT VERSION
    Works with RT 5.0.2, 5.0.3

### INSTALLATION
    perl Makefile.PL
    make
    make install
        May need root permissions

    Edit your /opt/rt4/etc/RT_SiteConfig.pm
        Add this line:

            Plugin('RT::Extension::ReplyWithMail');

    Clear your mason cache
            rm -rf /opt/rt5/var/mason_data/obj

    Restart your webserver

### AUTHOR
    Averkios

    All bugs should be reported via email to
        bug-RT-Extension-ReplyWithMail@rt.cpan.org
    or via the web at
        http://rt.cpan.org/Public/Dist/Display.html?Name=RT-Extension-ReplyWithMail
### LICENSE AND COPYRIGHT
    This software is Copyright (c) 2021 by Averkios

    This is free software, licensed under:

      The GNU General Public License, Version 2, June 1991

