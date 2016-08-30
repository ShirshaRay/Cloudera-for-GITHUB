1.Before Proceeding With CM installation through script,please verify all Pre-Requisite Steps.
2.Update Platform_Template.xml.
3.Go To /opt/cto/scripts and run below command:
    python setup_platform.py
    
    setup_platform.py script is going to do below jobs in the mentioned order:
    --------------------------------------------------------------------------
    1.Validation of RPMS :
        -->All the required rpms are installed or not.
    2.VALIDATION OF TEMPLATE XML FILE
        --> To check if Platform_template.xml is having all the required elements/subelements with correct property names.
    3.INSTALLATION OF PLATFORM BEGIN:
        -->Setting of Repo files to cloudera manager
        -->Installing Cloudera Manager Database
        -->Installing Database Connector
        -->Installing Cloudera Manager
        -->Creating Cloudera Manager Schema
        -->Installing packages on Cloudera Agents
        -->Deploying ZooKeeper
        -->Deploying HDFS Service
        -->Deploying YARN Service
        -->Deploying HBASE Service
        -->Deploying HIVE Service
        -->Starting Spark On Yarn Service
        -->Starting Thrift Server
        -->Enabling Kerberos
2.Go To /opt/cto/scripts and run below command:
    python updateHiveMetastore.py
    -->Postgres Hive Metastore Creation.
    
    