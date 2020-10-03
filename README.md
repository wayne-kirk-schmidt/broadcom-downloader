
Broadcom Download
=================

This is a small wrapper to manage the downloading, unpacking, and staging of broadcom log files

Installing the Scripts
=======================

Written in bash, this script is designed to be Unix agnostic and used in DevOps scripts.

You will need to use Bash 4+ as some of the scripts use associative arrays in the scripts.

Please follow the following steps to install:

    1. Download and install curl for your platform if you don't already have it installed.

       curl can be downloaded from https://curl.haxx.se/download.html

    2. Download and install git for your platform if you don't already have it installed.

       It can be downloaded from https://git-scm.com/downloads
    
    3. Open a new shell/command prompt. Change to the folder where you want to install the scripts.
    
    4. Clone this repo using the following command:
    
       git clone https://github.com/wks-sumo-logic/download_broadcom

       This will create a new folder.
    
    5. Change into the this folder. 

    6. Run the script:

       ./bin/broadcom_download -h

Use Case Usage
==============

1. To get the help page:

       ./bin/broadcom_download -h

2. To specify the credentials to be used [ needed ]

       ./download_import_files -k APIKEY:APISECRET

3. To specify the timerange to be used

       ./download_import_files -k APIKEY:APISECRET -t 12345667788987:124566788698

4. To specify the script to be used in verbose and debug mode

       ./download_import_files -k APIKEY:APISECRET -t 12345667788987:124566788698 -v -d

To Do List:
===========

* add a publish to a Sumo Logic Web endpoint

License
=======

Copyright 2020 Wayne Kirk Schmidt

Licensed under the GNU GPL License (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    license-name   GNU GPL
    license-url    http://www.gnu.org/licenses/gpl.html

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Support
=======

Feel free to e-mail me with issues to: wschmidt@sumologic.com
I will provide "best effort" fixes and extend the scripts.

