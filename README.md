# madgraph_pythia
This repo is for testing the magraph-pythia generated workflow.  

Use `./run.sh` to run yadage-workflow on workflow.yml  

workflow1.yml is a back-up version with the originally generated workflow.  

Current Bug:  
`2020-02-05 11:10:06,472 |   pack.madgraph.step |  ERROR | non-zero return code raising exception`  

`2020-02-05 11:10:06,472 |   pack.madgraph.step |  ERROR | subprocess failed. code: 1,  command docker run --rm -i  --cidfile /Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/generation_madgraph_pythia/madgraph/_packtivity/madgraph.cid     -v /Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/generation_madgraph_pythia/madgraph:/Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/generation_madgraph_pythia/madgraph:rw -v /Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/init:/Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/init:rw recast/madgraph:2.6.7 sh -c sh`
