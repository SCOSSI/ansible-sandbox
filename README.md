# ansible-sandbox

* ansible all -m ping -u vagrant --ask-pass

* ansible machine2 -m shell -a 'echo $TERM'

* ansible machine2 -m copy -a "src=/home/vagrant/test.txt dest=/home/vagrant" -u vagrant --ask-pass

* ansible machine2 -m apt -a "name=git" -sudo -u vagrant --ask-pass

* ansible machine2 -m git -a "repo=git://github.com/salerno-rafael/liquibase-sandbox.git dest=/home/vagrant/git_test version=HEAD" -u vagrant --ask-pass

* ansible-playbook playbook.yml -sudo -u vagrant --ask-pass