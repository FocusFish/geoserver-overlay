# geoserver-overlay

Repacks [geoserver](https://github.com/geoserver/geoserver/) adding UVMS specific
configuration.

Care must be taken when upgrading GeoServer since e.g. web.xml has been
modified and depending on the changes made in the new release will have to be
brought in to this repository as well. Failure to do so might result in
GeoServer not working as intended.

# Starting point

Uses [geoserver minimal](https://github.com/geoserver/geoserver/tree/main/data/minimal) as the base
and then adding UVMS specific changes (styling, workspaces, usm4uvms
AuthenticationFilter).

The base was chosen since it's an "empty" GeoServer data directory and is thus
not subject to a data license.
