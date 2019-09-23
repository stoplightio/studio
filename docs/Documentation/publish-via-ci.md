# Publish from Command Line 

> Preferred Method for Continuous Integration 

![Publish Via CLI](../../assets/images/publish-via-cli.png)

1. Install the @stoplight/cli package from NPM 

```
npm i -g @stoplight/cli

# The “stoplight” cli should now be available globally 

stoplight -h 
```

2. Make sure you are in the root directory of the local git repository associated with this project 

```
cd directory/to/analyze 
```

3. Run the analyze command, passing in the secret token associated with this project (the project token can be found in the project settings publish section). This will analyze all the design-related files in the local project directory, and send the information to Stoplight to be displayed as published docs, included in the search explorer, etc. 

```
stoplight analyze --token ************ 
```

> You can add the `--dry-run` flag to the analyze command to see what will be sent to Stoplight, without actually sending the data. 
