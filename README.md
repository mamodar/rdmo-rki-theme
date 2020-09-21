# RKI Theme for RDMO

This project tries to adapt the RKI theme used in the [datalinker](https://github.com/mamodar/datalinker) to RDMO.

## Install

1. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/configuration/themes.html#create-automatically) to generate the nessecary preconditions
2. Checkout this repository
3. Copy and overwrite all files in `rdmo-rki-theme/theme` to `rdmo-app/theme`
4. Copy and overwrite all files in `rdmo-rki-theme/local` to `rdmo-app/env/lib/python3.6/site-packages/rdmo/`
5. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/administration/site.html) to change *Display Name* and *Domain Name* to `RDMO`

Repeat step 2. and 3. whenever the theme is updated.
