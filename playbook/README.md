playbook uses only localhost with ssh connection type, and have 3 global tasks group:
1. Install Java.
  1.1. set variables $java_jdk_version, $java_oracle_jdk_package and $java_home
  1.2. upload Java binaries from local directory to /tmp/jdk-$java_jdk_version.tar.gz
  1.3. Ensure installation dir exists
  1.4. Extract java in the installation directory
  1.5. Export environment variables
"tags: java" is used for all tasks
2. Install Elasticsearch
  1.1. Set variables $elastic_version and $elastic_home
  1.2. Upload tar.gz Elasticsearch from remote URL
  1.3. Create directrory for Elasticsearch
  1.4. Extract Elasticsearch in the installation directory
  1.5. Set environment Elastic
"tags: elastic" is used for all tasks
3. Install Kibana
  1.1. Set variables $kibana_version and $kibana_home
  1.2. Upload tar.gz Kibana from remote URL
  1.3. Create directrory for Kibaan
  1.4. Extract Kibana in the installation directory
  1.5. Set environment Kibana
"tags: elastic" is used for all tasks

