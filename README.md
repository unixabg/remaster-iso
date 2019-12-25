# remaster-iso
Set of scripts to assist remastering an iso image with some custom settings for debian based systems.

## Generic steps would be something like the following:

    # clone the project
    git clone https://github.com/unixabg/remaster-iso.git

    # move to our remaster-iso directory
    cd remaster-iso

    # download the debian based iso we want to remaster
    wget http://somepath.blah/theIsoYouWant.iso

    # extract the iso
    remaster-extract -i theIsoYouWant.iso

    # make modifications to the squashfs things
    remaster-squashfs-editor

    # compose the iso back together
    remaster-compose
