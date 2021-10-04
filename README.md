# SPATIAL_MULTIMODEL

Follow the below steps with their corresponding videos:
  1. Setting up the SAP Business Application Studio
   
      Video 1 BAS Access and Configuration.mp4
    
  2. Import Catalog Objects into HANA Cloud
    
      Video 2 Catalog Import.mp4
    
  3. Set up of Pre-requisites for Spatial Project, Clone from the Git Repository and Deploy
      
      Video 3 Project Configuration and Deployment.mp4
    
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
    "password": "Demo2021",
    "port": "443",
    "tags": [
        "hana"
    ],
    "user": "UPS_SPATIAL_DATA_USER",
    "validate_certificate": false
    }
    
  4. Setup of Database User for SAC Development
    Video 4 Create SAC Database User.mp4
    
    Additional scripts needed:
    
    CREATE USER SAC_TRIAL_USER  PASSWORD "Demo2021!" NO FORCE_FIRST_PASSWORD_CHANGE; 
    
  5. Configure a Live Connection from SAC to HANA
    
      Video 5 HANA to SAC Live Data Connection.mp4
    
  6. Build and Visualize SAC Models based on HANA Database Objects
    
      Video 6 Create SAC Models and Stories.mp4


