## GRU Experimental Branch for: Self-Monitoring Navigation Agent for Vision-and-Language Navigation
In this branch I have made modifications to several files for incorporating GRU cells into the existing model's architecture.
There are also changes made for outputing the accuracy during testing to compare performance versus instruction length.    
Modified Files:  
  *tasks/R2R-pano/models/encoder.py  
    *The \__init\__ and forward methods were modified to include GRU cells. 
  *tasks/R2R-pano/main.py  
    *Added command line parameter for selecting GRU and instantiation of GRU based encoder.  
  *tasks/R2R-pano/agents/pano_agent.py  
    *Changes made for saving evaluation results. Added GRU functionality to rollout_monitor method.  
  *tasks/R2R-pano/models/policy_model.py  
    *The SelfMonitoring class \__init\__ and forward methods were modified to include GRU cells.  
  *tasks/R2R-pano/models/rnn.py  
    *The \_forward\_rnn and forward methods were modified to include GRU cells.  
  
The original project's README can be found [HERE](https://github.com/charlesramey/selfmonitoring-agent/blob/master/README.md).
