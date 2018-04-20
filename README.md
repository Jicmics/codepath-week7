# codepath-week7

# Project 7 - WordPress Pentesting

Time spent: 5 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Submit Comment XSS Vulnerability 
  - Summary: In WordPress before 4.2.2— user is allowed to submit malicious javascript in a comment box on any page. A standard example is just an alert box. Whenever someone now loads the main page, this alert box will pop up. 

    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1

    <img src="XSS_Submit_Comment" width="800">

2. Generic User Enumeration of WP-Login.php page
  - Summary: Allows the user to enumerate thru a list of valid usernames—— this is till a flaw in the code and the page should not specify whether usernames are valid or not. Someone with malicious intent could validate whether a user account exists and then attempt to brute force access.
    - Vulnerability types: USER ENUMERATION 
    - Tested in version: 4.2
    - Fixed in version: 4.3

    <img src="user_enumeration" width="800">

3. 
  - Summary: User must have permission to create and/or edit posts. Using the text tab, a user can submit a malicious script inside raw html code. A classic example is a hover over script as scene in the gif.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3

    <img src="XSS_Caption_Code" width="800">




## Assets


## Resources

sumofpwn.nl/advisory

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes



## License

    Copyright [2018] [Jacob Biller]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
