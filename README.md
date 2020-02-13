# madgraph_pythia
This repo is for testing the magraph-pythia generated workflow.  
  
Use `./run.sh` to run yadage-workflow on workflow.yml. 
Use `./clean.sh` to create a fresh workdir and copy proc_card_mg5.dat into wokdir/init to use it as input.  

workflow1.yml is a back-up version with the originally generated workflow.  
  
Current Bug:  
```
cwd=/code
ufotar=None
proc_card=/Users/vlad/Documents/EPEprojects/yadage-tests/madgraph_pythia/workdir/init/proc_card_mg5.dat
param_card=None
run_card=None
Traceback (most recent call last):
  File "steer_madgraph.py", line 75, in <module>
    main()
  File "steer_madgraph.py", line 71, in main
    args.param_card, args.run_card, args.shower_card, args.shower, args.n_events)
  File "steer_madgraph.py", line 50, in run_madgraph
    event_path = glob.glob(os.path.join(run_dir, '*.lhe.gz'))[0]
IndexError: list index out of range
```

## List of Changes Made to Generated Workflow
- removed unecessary parameters(param_card, run_card) from madgraph workflow
- manually copy input proc card into workflow/init
