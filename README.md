# RKI Theme for RDMO

This project tries improve the UI/UX of RDMO. It also adapts the RKI theme used in the [datalinker](https://github.com/mamodar/datalinker) to RDMO.

## Install

1. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/configuration/themes.html#create-automatically) to generate the necessary preconditions
2. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/administration/site.html) to change *Display Name* and *Domain Name* to `RDMO`
3. Checkout [this repository](https://github.com/mamodar/rdmo-rki-theme.git) 
4. Copy all files from `rdmo-rki-theme/theme` into `rdmo-app/theme`, overwrite
5. Copy all files from `rdmo-rki-theme/local` into `rdmo-app/env/lib/python3.6/site-packages/rdmo/`, overwrite


Repeat step 4. and 5. whenever the theme or RDMO is updated.
