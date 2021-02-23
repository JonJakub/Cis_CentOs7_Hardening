# Cis_CentOs7_Hardening
Cis_CentOs7_Hardening

ansible-playbook -i inventories/test.yml playbook.yml --private-key ~/.ssh/id_rsa  --user=jjon --ask-become-pass --check


inventories - treba doplnit servery na které je treba to aplikovat


skipovat se da dle sekci rhel7cis_section1/2/3/4/5/6

task/vars/main.yml jsou promene pro vsechny tasky zde se da podrobne ovladat co se pousti a co ne.
plus je treba definovat outputfiles: /root/   - kam se budou audtini ulohy ukladat
                         ssh_key_algorithms: example   - sifrovaci algoritmus ktery chceme pouzit


Dulezite:

4.2.1.5 Ensure rsyslog is configured to send logs to a remote log host

vars/main.yml:
remoteSyslog: example  - je treba doplnit




