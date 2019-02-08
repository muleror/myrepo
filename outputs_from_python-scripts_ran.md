(venv2) RMULERO-M-D3DH:samples rmulero$ python aci-show-subnets.py
Tenant      Application Profile Bridge Domain Subnet          Scope        
----------- ------------------- ------------- --------------- -------------
Demo1       demo1-App1          bd-1          2.2.2.1/24      private      
Demo2       demo1-App2          bd-2          3.3.3.1/24      private      
FTL-Lab-REY FTL_Lab_Apps        VLAN2         10.96.98.245/24 public,shared
FTL-Lab-REY FTL_Lab_Apps        VLAN96        10.96.96.8/24   public,shared
FTL-Lab-REY FTL_Lab_Apps        iSCSI_VLAN10  192.168.1.1/24  public,shared
ROCKS1      APP_ROCKS1          ROCKS1-BD                                  
ROCKS1      APP_ROCKS1          ROCKS2-BD                                  
common      default             default                                    
infra       access              ave-ctrl                                   
infra       access              default                                    
infra       ave-ctrl            ave-ctrl                                   
infra       ave-ctrl            default                                    
mgmt        VMWareAppProf       inb                                   


