## Export
Outputs:

  DBSecurityGroup:
    Description: A Reference To The Resource Id Of Security Group For Private Load Balancer
    Value: !Ref ContainerSG
    Export:
      Name: !Sub vm-managed-${EnvironmentParameter}-db-sg
      
      
## Import
Public_IP: 'Fn::ImportValue': !Sub "vm-managed-${EnvironmentParameter}-public-ip'
