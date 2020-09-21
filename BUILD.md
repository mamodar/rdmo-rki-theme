https://github.com/rdmorganiser/rdmo/blob/master/docs/i18n.md

OLD_ENG NEW_ENG
OLD_DE NEW_DE

~/rdmo-app$ source env/bin/activate

Find file FILE which contains OLD_ENG in ~/rdmo-app/env/lib/python3.6/site-packages/rdmo
Backup FILE to FILE_BACKUP
replace OLD_ENG by NEW_ENG
Copy FILE to theme folder (FILE has to be the same in ~/rdmo-app/env/lib/python3.6/site-packages/rdmo and  ~/rdmo-app/theme/templates/ )

nano ~/rdmo-app/env/lib/python3.6/site-packages/rdmo/locale/de/LC_MESSAGES/django.po
look for the OLD_ENG, replace it by NEW_ENG
replace OLD_DE by NEW_DE

cd ~/rdmo-app/env/lib/python3.6/site-packages/rdmo
django-admin makemessages
django-admin compilemessages

OPTIONAL: replace FILE in original location by FILE_BACKUP

Do not espace quotation marks in FILE but only in djano.po
