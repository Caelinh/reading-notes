# Amplfy and cognito

## Authentication with amplify
- Cognito is AWS authentication system
- to use auth it needs to be added to the project
````
amplify add auth
````
````
? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`
````
Then push changes to the cloud with ````amplify push````
 - Add dependencies
 ````
 dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.37.3'
}
````
**DOCS** - https://docs.amplify.aws/lib/auth/getting-started/q/platform/android/#install-amplify-libraries  

## Signing in the user
All steps for signing in can be found [here](https://docs.amplify.aws/lib/auth/signin/q/platform/android/#multi-factor-authentication)  
- users can sign up with email and also receive sms texts for authentication.  

