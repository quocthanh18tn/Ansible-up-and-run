lession1: Virtualenv pip
pip: bo quan ly cac package cua python, quan ly cac framework ,lib khac viet = python.
ansile: cac module viet = python, co the viet nhieu = ngon ngu khac, nhu python supports nhieu nhat.
ansbile: chi la thuc thi nhung cai command minh truyen vao thoi.
- setup:
  pip install virtualenv
sau khi c
  mkdir folder
  virtualenv < variable >  ex:virtualenv project1_env
                              source project1_env

pip install virtualenv
mkdir folder
. ./folder/bin/activate
pip install cai gi do
pip freeze --local requirement.txt
pip install -r requirement.txt


git add abc.txt
git commit -m "abc"

git add abc.txt2
git commit --amend --no-edit

// tuc la gop 2 cai lai 1

git commit --amend --no-edit -m "bacded"

//thoi doi committ thanh bacded gom co 2 file

git reset HEAD~1   //quay nguoc lai 1 commit truoc do


khi cau hinh chay vagrant k co ssh_key=false, thi vagrant se tu dong sinh key ra, khi do ping thi phai insert bien var chen key vao

[all:vars]
ansible_user=vagrant
ansible_ssh_private_key_file=./.vagrant/machines/default/virtualbox/private_key


con neu vagrant co ssh_key=flase thi vagrant se khong sinh key, minh phai xai key goc cua minh
[all:vars]
ansible_user=vagrant
ansible_ssh_private_key_file=~/.vagrant.d/insecure_private_key

ansible -i hosts all -m ping ( phai co -i hosts de no biet file nao)

ansible-playbook web-notls.yml -i hosts -> truy vao cap localhost:8080 se ra