DEPRECATED, USE CMSSW FORK INSTEAD
https://twiki.cern.ch/twiki/bin/viewauth/CMS/HiForestSetup

HiForestSetup
=======================

Scripts to setup the HiForestProduction areas


Create a new, clean area using the correct CMSSW version (currently CMSSW_5_3_8_HI_patch2 for pPb and 2013 pp). Check out the latest version of the forest setup script and run it to prepare the foresting area.

    cmsrel CMSSW_5_3_8_HI_patch2
    cd CMSSW_5_3_8_HI_patch2
    cmsenv
    git clone git@github.com:CmsHI/HiForestSetup.git
    cd src/
    ../HiForestSetup/setup_hiForest2_538_git.sh

The last command may take ~5 minutes to finish checking out all the code and compiling it. If there are ANY errors which halt compilation, please report them to the hn-cms-hi-general list and check in to CVS/git any changes you make to fix errors.

Foresting configurations reside in https://github.com/CmsHI/HiForestProduction/tree/master/ForestConfigurations (or in the folder ForestConfigurations if you follow these directions). Different branches have different configurations available - please check the branch appropriate for your needs. The naming convention should tell you what sample each configuration is intended for. 
