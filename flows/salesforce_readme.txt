1. Copy the variables from salesforce_env.yaml into <sequor_env_dir>/variables.yaml and fill in the values of the variables.

2. salesforce_client_id and salesforce_client_secret represent consumer_id and consumer_secret of your "Connected app" in Salesforce. 
For instructions, search online or prompt an AI: how to create connected app in Salesforce.

3. salesforce_password is constructed by concatinating your password with user personal security token. 
To get the token: log in to Salesforce, go to <your name> > My Settings > Personal  >  Reset My Security Token. 
It will be sent to you via email.
