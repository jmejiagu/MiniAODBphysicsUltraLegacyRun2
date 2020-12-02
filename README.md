# MiniAODBphysicsUltraLegacyRun2

## Intructions to run the examples.
```
source /cvmfs/cms.cern.ch/cmsset_default.sh
cmsrel CMSSW_10_6_12
cd CMSSW_10_6_12/src/
cmsenv
voms-proxy-init -voms cms -valid 192:00
git clone https://github.com/jmejiagu/MiniAODBphysicsUltraLegacyRun2.git myAnalyzers/JPsiKsPAT
cd myAnalyzers/JPsiKsPAT/
git checkout master
cd ../..
scram b
cd myAnalyzers/JPsiKsPAT/test/
cmsRun PsikaonRootupler.py
```