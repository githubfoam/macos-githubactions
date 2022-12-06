# macos-githubactions

[![.github/workflows/macos-osquery-workflow.yml](https://github.com/githubfoam/macos-githubactions/actions/workflows/macos-osquery-workflow.yml/badge.svg?branch=main)](https://github.com/githubfoam/macos-githubactions/actions/workflows/macos-osquery-workflow.yml)  
[![matrix java macos CI workflow](https://github.com/githubfoam/macos-githubactions/actions/workflows/jdk-matrix-wf.yml/badge.svg)](https://github.com/githubfoam/macos-githubactions/actions/workflows/jdk-matrix-wf.yml)

CTI, DFIR, OSX
~~~~
Finding specific indicators of compromise (IOCs) in memory or on disk; Facebook has provided the queries which detect Hacking Team’s OSX backdoor by querying for specific persistent mechanisms and file system activity on OSX

select * from file where path = '/dev/ptmx0';
select * from apps where bundle_identifier = 'com.ht.RCSMac' or bundle_identifier like 'com.yourcompany.%' or bundle_package_type like 'OSAX';
select * from launchd where label = 'com.ht.RCSMac' or label like 'com.yourcompany.%' or name = 'com.apple.loginStoreagent.plist' or name = 'com.apple.mdworker.plist' or name = 'com.apple.UIServerLogin.plist';


~~~~
~~~~
macos_osquery 
https://gist.github.com/githubfoam/6753b5efad8e5ab8fa2ca29ce7b29988
windows_osquery 
https://gist.github.com/githubfoam/afeb4fbbee731c427d645382e59b7948
linux_osquery 
https://gist.github.com/githubfoam/0babb95da5845b8d4ee41f5711de637a
~~~~

~~~~
predefined tables
<https://osquery.io/schema/4.1.1>

# https://osquery.readthedocs.io/en/stable/installation/install-linux/

https://github.com/google/santa
https://github.com/groob/moroz
https://github.com/zentralopensource/zentral

~~~~

~~~~
https://github.com/actions/runner-images
~~~~