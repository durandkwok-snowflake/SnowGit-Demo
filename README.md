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

**Note: You have the options of using secrets for the api integration.**

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

<img width="572" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/4391eff9-720f-46c8-8934-8d9b57821a0b">

### Enter Repository Name
<img width="494" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/5611293a-83cb-4576-a630-deeb91ce8bca">

### Enter Origin
#### Fetch the URL from the Github you want to integrate with

<img width="493" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/9ed4517a-8c58-4698-98d8-5eed3a410971">

#### and populate the Origin field from Setup

<img width="480" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/6c72bf44-626d-4ec9-81bf-414962814307">

#### Select the API Integration from the drop down list

<img width="499" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/41f592fc-c97b-420c-9490-56fb3566a962">

#### Select Enable Authentication if your repository is private (Note: My repository is public therefore I did not enable authentication)

<img width="500" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/b5e7e46b-d104-421b-a4b5-92c33f3c18f2">

#### The setup should look something like this

<img width="502" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/0a603ec3-2e49-4b8e-bed9-62c292d83239">

### Select Create to proceed

<img width="144" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/54926133-3459-4306-84e9-f01f1b30d816">

### Navigate to the newly create Git Repository
<img width="1426" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/2dfea976-4ce6-480a-9a07-dd41022d5cb9">

### You should be able to see the contents of your repository. From the repository, you are able to execute immediately, copy the content into a new worksheet, copy the path or download
<img width="1141" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/3859d996-ccf5-4674-93ea-f6ad3a8d3b95">

### Testing with copy into worksheet

<img width="1256" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/d957cca9-dcde-4034-92ec-8ad0f37f55ca">








