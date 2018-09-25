# Assorted Plone Scripts

This repository contains a number of maintenance scripts that have been used by Zest Software over the years while supporting Plone sites for customers.

We don't claim ownership of these, some have been written by us, some were
found in gists or elsewhere. When we know the origin of a script its listed
below at each scripts's description and usage info. If we have missed any
attribution, please contact us at info@zestsoftware.nl

Most scripts should be started from the command line by using

> bin/instance run ./path/to/script.py --paramaters

For some it also seems possible to run in a zeoclient/zeoserver setup, but
do reaalise that you could run into ZODB conflict errors an degraded results if the database is also written to by other zeoclients.

## purge_image_scales.py

Created by Maurits van Rees, Zest Software. This script is used to remove all images scales from objects in a plone site created by plone.scale. When you change available scales in your site, old scales will persist on the object. It is however safe to remove all of them because they will be autogenerated again.
