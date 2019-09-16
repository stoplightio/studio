# Publish from Command Line 

![]()

1. Install the @stoplight/cli package from NPM 

```
Npm i -g @stoplight/cli

# The “stoplight” cli should now be available globally 

Stoplight help 
```

2. Make sure you are in the root directory of the local git repository associated with this project 

```
cd directory/to/analyze 
```

3. Run the analyze command, passing in the secret token associated with this project, and the Stoplight API host. This will analyze all the design-related files in the local project directory, and send the information to Stoplight to be displayed as published docs, included in the search explorer, etc. 

```
stoplight analyze --token ************ --api-host https://stoplight.io/api 
```

> You can add the `--dry-run` flag to the analyze command to see what will be sent to Stoplight, without actually sending the data. 
