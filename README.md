# SnowGit-Setup
## With SnowGit read-only in Snowsight user can now:

*Connect to an existing git repository via the Create object → Git Repository flow in the UI

*See all their branches, tags and folders and files inside their repository

*Fetch the latest version of their files via the UI

*Execute immediate SQL files directly from the repo (after seeing a code-preview)

*Copy the path to a repo file to be used in a script or app or notebook

*Copy the code from a SQL-script template into a worksheet to modify and run it

*Download a file from the repo to use it locally
### Create API INTEGRATION

<img width="1235" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/3f63db31-5e8f-476b-bede-c9cc596c7758">

```SQL
CREATE OR REPLACE API INTEGRATION git_api_integration_scaling_test
  API_PROVIDER = git_https_api
  API_ALLOWED_PREFIXES = ('https://github.com/durandkwok-snowflake/DK_Snowflake_Scaling_Compute_Demo.git')
  --ALLOWED_AUTHENTICATION_SECRETS = (git_secret)
  ENABLED = TRUE;
```
### Select a Database and Schema to Create Git Repository Integration
<img width="275" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/def78c08-3756-4fc6-adc1-dcd205e9298a">

<img width="1147" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/1a02b83d-9372-4002-85c9-1faeaebf6892">

<img width="183" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/2f45b58a-cd60-4b88-94bb-52a34be05896">

<img width="572" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/4391eff9-720f-46c8-8934-8d9b57821a0b">


### Enter Repository Name
<img width="494" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/5611293a-83cb-4576-a630-deeb91ce8bca">

### Enter Origin
#### Fetch the URL from the Github you want to integrate with

<img width="507" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/9795d690-2f52-46b9-b5da-dfd562638e32">

#### and populate the Origin field

<img width="480" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/6c72bf44-626d-4ec9-81bf-414962814307">


<img width="502" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/0a603ec3-2e49-4b8e-bed9-62c292d83239">

