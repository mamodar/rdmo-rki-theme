# RKI Theme for RDMO

This project aims at  improving the UI and UX of RDMO. It also adapts the RKI theme used in the [datalinker](https://github.com/mamodar/datalinker) to RDMO.

## Install
1. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/configuration/themes.html#create-automatically) to enable the support for themes
2. Follow the [RDMO documentation](https://rdmo.readthedocs.io/en/latest/administration/site.html) to change *Display Name* and *Domain Name* to `RDMO`
3. Checkout [this repository](https://github.com/mamodar/rdmo-rki-theme.git) on your machine   
     1. Check if the version in [VERSION](VERSION) matches the RDMO version   
     1. Otherwise, checkout the correct tag from the repository   
4. Remove all files in `rdmo-app/theme`
5. Copy all files from `rdmo-rki-theme/theme` into `rdmo-app/theme`, overwrite
6. Copy all files from `rdmo-rki-theme/local` into `rdmo-app/env/lib/python3.6/site-packages/rdmo/local`, overwrite
7. Copy all files from `rdmo-rki-theme/projects` into `rdmo-app/env/lib/python3.6/site-packages/rdmo/projects`, overwrite


Repeat step 3. to 7. whenever the theme or RDMO is updated.
