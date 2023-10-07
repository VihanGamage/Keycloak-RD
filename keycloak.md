Customize keycloak welcome & admin themes
=========================================

To install keycloak lastest version 22.0.3 on Ubuntu:

    https://www.keycloak.org/downloads

To extract the pre-built themes you need to go to this path

    ..lib/lib/main/org.keycloak.keycloak-themes-22.0.3

To create new customized themes in Keycloak: 
    
    create a new folder in themes directory, let’s call it mytheme

To change the welcome page:

    create a welcome folder inside the mytheme folder.Then change the logo and heading of the welcome page.And remove the documentation, keycloak project, mailing list and report issue components


To change the admin console page logo :

    create a admin folder inside the mytheme folder. Then add a new logo to the theme.properties file.

To start the keycloak server run this command :

    sudo bin/kc.sh start-dev --spi-theme-welcome-theme=mytheme


After the server boots, open http://localhost:8080 in your web browser. The welcome page will indicate that the server is running.
