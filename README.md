
Broadcom Download
=================

This is a wrapper to download, stage, and publish Broadcom log files to Sumo Logic

Installing the Scripts
=======================

Written in bash, this script is designed to be Unix agnostic and used in DevOps scripts.

Please ensure you have at least version 4+ of Bash installed

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

    6. See how to run the script in the "Common Usage"

Preparation
===========

This script can be run by itself or in conjunction with an installed collector.
If you want to do this, you will need to install:

1. An hosted collector

   https://help.sumologic.com/03Send-Data/Hosted-Collectors

2. An web source

   https://help.sumologic.com/03Send-Data/Sources/02Sources-for-Hosted-Collectors

3. Installed collector with a Script Source to run the script

   https://help.sumologic.com/03Send-Data/Installed-Collectors

   https://help.sumologic.com/03Send-Data/Sources/01Sources-for-Installed-Collectors/Script-Source

Common Usage
============

1. To get the help page:

       ./bin/broadcom_download -h

2. To specify the credentials to be used [ needed ]

       ./download_broadcom -k APIKEY:APISECRET

3. To specify the timerange to be used

       ./download_broadcom -k APIKEY:APISECRET -t 12345667788987:124566788698

4. To specify the script to be used in verbose and debug mode

       ./download_broadcom -k APIKEY:APISECRET -t 12345667788987:124566788698 -v

5. To publish the contents of the Broadcom logs to a Sumo Logic Web HTTP Endpoint

       ./download_broadcom -k APIKEY:APISECRET -t 12345667788987:124566788698 -v \
         -w https://collectors.jp.sumologic.com/receiver/v1/http/<endpointaddress>

To Do List:
===========

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

