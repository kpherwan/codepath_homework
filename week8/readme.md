# Project 7 - WordPress Pentesting

Time spent: 3 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. (Required) Vulnerability Name or ID
  - [ ] Summary: Part of testing created various accounts, and in scenarios where a person tried to login with default credentials or any username or password the error is specific and provides details on whether username or password right or wrong. 
    - Vulnerability types: User Enumeration (CVE-2020-7918)
    - Tested in version: version 4.0 
  - [ ] GIF Walkthrough: https://github.com/kpherwan/codepath_homework/blob/main/week8/2022-04-17%2015.54.14.gif
  - [ ] Steps to recreate:  made a account in our wordpress, when a person tried to login and tried several username and at last he found that admin username exist
  - [ ] Affected source code:
    - [Link 1](http://wpdistillery.vm/wp-login.php)

### 2. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types: Password enumeration
    - Tested in version: 4.1
  - [ ] GIF Walkthrough: https://github.com/kpherwan/codepath_homework/blob/main/week8/2022-04-17%2017.13.07.gif
  - [ ] Steps to recreate: Ran the scan command wpscan --url http://127.0.0.1:8080 --usernames username.txt --passwords password.txt with usernames from previous scan and passwords from the list of popular passwords found on the internet
  
### 3. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:  Unauthenticated Stored Cross-Site Scripting (XSS)
    - Tested in version: 4.1
    - Fixed in version: 4.1.2
  - [ ] GIF Walkthrough: https://github.com/kpherwan/codepath_homework/blob/main/week8/2022-04-17%2017.41.06.gif
  - [ ] Steps to recreate: Tried cross site scripting in main body and comment, and comment section does not seem to be sanitized
 
### 4. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
