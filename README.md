# project1
# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) WordPress <= 4.3 - Authenticated Shortcode Tags Cross-Site Scripting (XSS)
  - [ ] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.3.1
  - [ ] GIF Walkthrough: https://i.imgur.com/B5dvyNA.gif
  - [ ] Steps to recreate: Post”TEST!!![caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">Click me</a>,then come to the page, it will have a prompt
  - [ ] Affected source code:
    - [Link 1]	https://wordpress.org/news/2015/09/wordpress-4-3-1/
2. (Required) WordPress 2.5-4.6 - Authenticated Stored Cross-Site Scripting via Image Filename
  - [ ] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.6.1
  - [ ] GIF Walkthrough: https://i.imgur.com/D4Q9wTr.gif
  - [ ] Steps to recreate: Change the name of a screenshot to ><svg onload=alert(1)>.png, then upload it to the Media section, view the property of the image, same prompt shows up.
  - [ ] Affected source code:
    - [Link 1] https://wordpress.org/news/2016/09/wordpress-4-6-1-security-and-maintenance-release/ 
3. (Optional) WordPress 2.3-4.3 - Authenticated Stored Cross-Site Scripting via comment
  - [ ] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.3.6
  - [ ] GIF Walkthrough: https://i.imgur.com/TzIscSP.gif
  - [ ] Steps to recreate: Post a comment of “<script>alert(1)</script>” then prompt of “1” shows up.
  - [ ] Affected source code:
    - [Link 1]	https://github.com/WordPress/WordPress/commit/70128fe7605cb963a46815cf91b0a5934f70eff5


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
