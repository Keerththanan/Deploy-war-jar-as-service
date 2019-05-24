# Deploy-war-jar-as-service

1. Go to your deployment directory
2. You should have 4 files which is mentioned below
    - Your jar/war
    - application.properties of the particular springboot application
    - WinSW.NET4.xml, where 
      - id -> The unique id of the sevice
      - name -> Name of the service
      - arguments -> -Dspring.config.location=application.properties -jar %Base%\leave.war
        - where last part should be your war/jar file name.
    - Finaly WinSW.NET4.exe file
3. Finally **in your service installation directory** type the below command
    - WinSW.NET4.exe install

## You are all done

If you want to remove the installed service, use this command
    - WinSW.NET4.exe uninstall

If you already installed same service with different name, change <id></id> in the xml file and then re run the uninstallation command.
---


    
