# Cis_CentOs7_Hardening
Cis_CentOs7_Hardening

ansible-playbook -i inventories/test.yml playbook.yml --private-key ~/.ssh/id_rsa  --user=jjon --ask-become-pass --check


inventories - treba doplnit servery na které je treba to aplikovat
Momentalne tam je test.yml ve kterem je fincetrum ktere jsem pouzil na zouseni zda se to tam pusti a prode v rezimu --check


skipovat se da dle sekci rhel7cis_section1/2/3/4/5/6

task/vars/main.yml jsou promene pro vsechny tasky zde se da podrobne ovladat co se pousti a co ne.
plus je treba definovat outputfiles: /root/   - kam se budou audtini ulohy ukladat
                         


Variables k doplneni

vars/main.yml:
remoteSyslog  - je treba doplnit
rhel7cis_rule_5_2_15 by defaul disabled - variables rhel7cis_sshd needs to be setup
ssh_key_algorithms: example   - sifrovaci algoritmus ktery chceme pouzit




