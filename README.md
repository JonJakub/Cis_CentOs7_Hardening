# Cis_CentOs7_Hardening
Cis_CentOs7_Hardening

ansible-playbook -i inventories/test.yml playbook.yml --private-key ~/.ssh/id_rsa  --user=jjon --ask-become-pass --check


inventories - treba doplnit servery na které je treba to aplikovat
Momentalne tam je test.yml ve kterem je fincetrum ktere jsem pouzil na zouseni zda se to tam pusti a prode v rezimu --check


 skipovat se da dle sekci rhel7cis_section1/2/3/4/5/6
                         


 Variables k doplneni

 task/vars/main.yml:

- remoteSyslog  - je treba doplnit
- rhel7cis_rule_5_2_15 by defaul disabled - treba nastavit rhel7cis_sshd nez se toto bude posutet
- ssh_key_algorithms: example   - sifrovaci algoritmus ktery chceme pouzit
-  outputfiles - vystup z auditnich tasku




