# SPATIAL_MULTIMODEL

Follow the below steps with their corresponding videos:
  1. Mission Architecture Review
    
        MISSION INTRODUCTION.mp4
    
  2. Import the schema into HANA Cloud
    
        IMPORT CATALOG OBJECTS.mp4
    
  3. Configure and deploy GIT repositories in Business Application Studio
      
        CONFIGURE and DEPLOY GIT REPOSITORY IN HANA CLOUD.mp4
    
    Additional scripts needed: 
    
    CREATE USER UPS_SPATIAL_DATA_USER  PASSWORD "Demo2021!" NO FORCE_FIRST_PASSWORD_CHANGE;
    GRANT SELECT , EXECUTE , SELECT METADATA , CREATE ANY  ON SCHEMA SPATIAL_DATA TO 
    UPS_SPATIAL_DATA_USER WITH GRANT OPTION;
    
    User Provided Service Name: UPS_SPATIAL_DEVELOPMENT
    JSON syntax for User Provided Service: 
    {
    "driver": "com.sap.db.jdbc.Driver",
    "encrypt": true,
    "endpoint": "https://api.cf.us10.hana.ondemand.com",
    "host": "You HANA host from HANA Cloud Cockpit",
    "password": "Demo2021!",
    "port": "443",
    "tags": [
        "hana"
    ],
    "user": "UPS_SPATIAL_DATA_USER",
    "validate_certificate": false
    }
    
  4. Create a SAP Analytics Cloud user and assign a role

        CREATE SAC USER and ASSIGN ROLES.mp4
   
    Additional scripts needed:
    
    CREATE USER SAC_TRIAL_USER  PASSWORD "Demo2021!" NO FORCE_FIRST_PASSWORD_CHANGE; 
    
  5. Create a live data connection from HANA Cloud to SAP Analytics Cloud
    
        LIVE HANA CLOUD CONNECTION IN SAC.mp4
    
  6. Build a data model and story in SAP Analytics Cloud for the truck trips scenario
    
      TRUCK TRIPS SAC MODEL AND STORY.mp4

  7. Build a data model and story in SAP Analytics Cloud for the fire burning scenario
    
      FIRE BURNING LOCATOINS SAC MODEL AND STORY.mp4

