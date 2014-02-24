fastTnPforPromptRate
====================

macro to perform TnP fits for prompt rate computation

How to use it:

-> prepare the histograms to fit:
 root -l -b -q 'makeHistos.C("/afs/cern.ch/work/a/albertog/public/pourHugues/TreeAnalysisStop_PR_DataMu12_Run2012ABCD.root")'

-> create the directory to store the fit plots:
mkdir fitPlots 

-> now fit the histograms:
root -b -q -l 'performTheFitsMuons.C("data")'

-> the TH2F containing the SF will appear in efficencyMuonsdata.root
