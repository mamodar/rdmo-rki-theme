https://github.com/rdmorganiser/rdmo/blob/master/docs/i18n.md
# Change the locale 

## Variables
OLD_ENG The original string in english (we want to replace this string)  
NEW_ENG The new string in english  
OLD_DE The original string in german  
NEW_DE The new string in german  

## How to

1. `source ~/rdmo-app/env/bin/activate`
2. Find file FILE which contains OLD_ENG in `~/rdmo-app/env/lib/python3.6/site-packages/rdmo`

   2. Backup FILE into FILEBACKUP
   2. replace OLD_ENG by NEW_ENG in FILE
   2. If you cannot find FILE, check if you can find OLD_ENG in the RDMO template folder
        2. In this case copy the template file from the template folder and replace FILE by it after the backup

3. Sync FILE into the template folder 
    3. Copy FILE to the theme folder of RDMO
    3. as a result FILE is the same in `~/rdmo-app/env/lib/python3.6/site-packages/rdmo/...` and  `~/rdmo-app/theme/...` 
    3. if the theme folder already includes FILE, merge these two files (**do not overwrite**)

4. Update locale
    4. Open the *django.po* locale file in the RDMO installation (`~/rdmo-app/env/lib/python3.6/site-packages/rdmo/locale/de/LC_MESSAGES/django.po`)
   4. replace OLD_ENG by NEW_ENG
   4. replace OLD_DE by NEW_DE

5. Build new locale
    5. Change to the main directory `cd ~/rdmo-app/env/lib/python3.6/site-packages/rdmo`
    5. `django-admin makemessages`
    5. `django-admin compilemessages`

6. Copy all changes files to this project
    6. Copy FILE from `~/rdmo-app/theme/...` into `~/rdmo-rki-theme/theme/...`
    6. Copy *django.po* **and** *django.mo* locale into `~/rdmo-rki.theme/locale/...` 
    6. Replace FILE by FILEBACKUP

Do not espace quotation marks in FILE but only in *djano.po*
