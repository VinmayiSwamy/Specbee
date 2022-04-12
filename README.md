# Specbee

### Story

As a user, I should be able to see the Site location and the current time for the location.


### Implementation details

   * Added an ADMIN CONFIGURATION form which will take the following inputs:
   * 
         Country - text field
         City - text field
         Timezone - select list
                Options in the select list
                America/Chicago
                America/New_York
                Asia/Tokyo
                Asia/Dubai
                Asia/Kolkata
                Europe/Amsterdam
                Europe/Oslo
                Europe/London
   * Created a service that will return the current time based on the time zone selection in the above form. Time will be in the format 25th Oct 2019 - 10:30 PM
   * Added a Plugin block that will render the Location from the configuration set in the ACF and the current time calling the service in the previous step. Passed the variables to a template to be rendered.
   
### Installing

* Please clone this module inside module/custom folder
* Then enable this module from the /admin/modules page

### Executing program
* Navigate to /admin/config/specbee_location/adminsettings or you can find config form link in /admin/config/ also with the tittle "Specbee Location configuration".
* 
  ![Alt text](images/config.png?raw=true "Config")
  
  ![Alt text](images/config_form.png?raw=true "ACF")
  
* Navigate to /admin/structure/block
* Place the Location time block in the content region and save it
* 
  ![Alt text](images/block.png?raw=true "Specbee Block")

### Output
  ![Alt text](images/output.png?raw=true "Output")
