# CowinHelpBot
COWIN help bot is designed to find available vaccinations in India from COWIN Portal.COWIN help bot makes use of COWIN API from API SETU. 

Algorithm :
1. Fetches All the district codes and district names and store them in an output file.
2. Clear column EmailSent and NoVaccineAvailable columns of output file (user details sheet) everyday at 9:00 am
3. Fetches any new entry for registration or unsubscribbing from Microsoft registration Form (URL in config)
4. Update the above details in output file and group the user details based on district name and age limit.
5. Search for any vaccine available slots in a particular district and send appropriate emails to the users.
6. If vaccines are available then send the details of the vaccine slots in email and update EmailSent column as Yes.
7. If vaccines are not available then send "no vaccine slots available" in email and update NoVaccineAvailable as Yes.
