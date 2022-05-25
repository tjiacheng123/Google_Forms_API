# Google_Forms_API
Just to provide some background on the rationale for creating a Google Forms API. My mother operates a drink stall but she is illiterate in the English language. She relies on me to be the 'procurement officer' of her stall. Every week, she sends me a list of canned drinks order(coke, 100 plus, ice lemon tea etc.) through text in Chinese. On my end, I will translate her orders into English and forward it via text to the vendor. The translation takes up about 10 to 15 mins a week and it would take even lesser time if I could automate the process.

  Step 1: Create a Chinese canned drinks order form on Google Form
  Step 2: Use Google Forms API to retrieve the latest form response
  Step 3: Use Python to translate the orders from Chinese to English and perform data transformation
  Step 4: Output the orders in a proper format for the vendor

Before writing the python script, I have configured APIs, set up authentication, and manage deployments on Google Cloud Platform. The set up includes:

1. Creating a Google Cloud project
2. Enabling the APIs to use in the Google Cloud project
3. Configuring OAuth consent
4. Creating access credentials to authenticate the app's end users or service accounts

The python script performs the following function:

1. Use Google Forms API to retrieve the form response and form metadata
2. Extracting the necessary information from dictionaries nested within lists
3. Data transformation
4. Exporting the final order to a txt file
