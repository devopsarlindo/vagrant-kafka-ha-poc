1. Run "vagrant up" to provision centos 7.2 servers

2. Install and Configure Kafka/Zookeeper on servers

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/deploykafka.yml

3. Restart Whole Clusters Kafka/Zookeeper

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/restartkafka.yml

4. Fail over to dc1

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/dcfailover_to_dc1.yml

5. Fail over to dc2

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/dcfailover_to_dc2.yml

6. Restore cluster back to normal state

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/dcfailover_restore_back_to_normal.yml

7. Run tests

ansible-playbook -i inventory/vagrant/hosts.ini playbooks/kafkatests.yml
