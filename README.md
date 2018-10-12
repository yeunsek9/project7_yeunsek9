# Project 7 - WordPress Pentesting

Time spent: **10** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Vulnerability Name or ID
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.3
  - [x] GIF Walkthrough: https://github.com/yeunsek9/test/raw/master/XSS1_yeunsek9.gif
  - [x] Steps to recreate: 1) Create new post
                           2) Add href="</a><a title=" onmouseover=alert('test') using the text edit.
         		   3) publish.
        		   4) Test will pop up.
  - [x] Affected source code:
  -[Reference](https://klikki.fi/adv/wordpress3.html)

1. (Required) Vulnerability Name or ID
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.6
  - [x] GIF Walkthrough: https://github.com/yeunsek9/test/raw/master/XSS2_yeunsek9.gif
  - [x] Steps to recreate: 1) make new post
         		   2) put script with url containing \x3c (escape code sequence <) followed by xss code and ending with \x3e (>).
  - [x] Affected source code:
  -[Reference](https://guides.codepath.com/websecurity/Cross-Site-Scripting)

1. (Required) Vulnerability Name or ID
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.3.1
  - [x] GIF Walkthrough: https://github.com/yeunsek9/test/raw/master/XSS3_yeunsek9.gif
  - [x] Steps to recreate: 1) put a comment, http://www.example.com/wp-admin/customize.php?theme=<svg onload=alert(1)>
         		   2) Alert will pop up
  - [x] Affected source code:
  -[Reference](https://wpvulndb.com/vulnerabilities/8358)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2018] [Eun Suk Lee]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.