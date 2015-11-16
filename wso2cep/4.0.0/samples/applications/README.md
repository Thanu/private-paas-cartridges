WSO2CEP-4.0.0 Application
=========================
A simple application with a wso2cep-4.0.0 cartridge.

Application view
----------------
wso2cep-4.0.0-app            <br />
-- wso2cep-4.0.0-app-1       <br />
-- -- wso2cep-4.0.0          <br />

Application folder structure
----------------------------
-- artifacts/[iaas]/ IaaS specific artifacts                <br />
-- scripts/common/ Common scripts for all iaases            <br />
-- scripts/[iaas] IaaS specific scripts                     <br />

How to run
----------
cd scripts/[iaas]/          <br />
./deploy.sh                 <br />

How to undeploy
---------------
cd scripts/[iaas]/          <br />
./undeploy.sh               <br />