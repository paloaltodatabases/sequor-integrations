1. Copy the variables from mailchimp_env.yaml into <sequor_env_dir>/variables.yaml and fill in the values of the variables.
2. You can find instructions on creating API key at https://mailchimp.com/developer/marketing/guides/quick-start/
3. Here is a link to the docs of Marketing API that we use in our examples: https://mailchimp.com/developer/marketing/api/

Run mailchimp_fetch_subscribers flow first as it creates mailchimp_subscribers table used in mailchimp_create_segment flow.