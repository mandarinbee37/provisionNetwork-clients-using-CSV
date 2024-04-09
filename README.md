Use the Meraki API call, provisionNetworkClients, to provision devices using their MAC Address and a friendly name, by importing information from a CSV file.

For this script we require that the following libraries are imported: import meraki import csv import os from dotenv import load_dotenv

This script uses dotenv to load environment variables. These can be added to an .env script in the same directory the python script is running in, added to configurations in an IDE like Pycharm, or exported directly from terminal.

If using terminal use the following syntax: export MERAKI_API_KEY=<API_KEY>. You will also need to export your NETWORK_ID.

The CSV file needs to contain the MAC Address of the device and a friendly name. Please note the row index.

![image](https://github.com/mandarinbee37/provisionNetwork-clients-using-CSV/assets/166555204/cb998d28-9106-41db-8855-589aa54f7342)

For example, the MAC Address field is row[0] and the name field is row[3] in this case (and in the script). You will need to manually adjust the row index for this script by editing it.
