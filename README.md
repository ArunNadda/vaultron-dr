### Vaultron DR cluster

- This repo is copy of vaultron (https://github.com/brianshumate/vaultron), with some changes to create additional cluster to check/test vault replication.
- for information on how to setup cluster please refer to readme of https://github.com/brianshumate/vaultron

### changes done:
- only changes are done for `raft` storage related setup, Thus consul storage setup will not work.
- changed `black_lion/main.tf` to modify docker instance names, IP addresses of vault instances from `vaultron-vault?` to `vaultrondr-vault?`, IP address from `10.10.42.20x` to `10.10.42.22x` and external port changed from `82xx` to `92xx`.
- certificates/ca-certs files are changed to accomodate new IP Addresses (`black_lion/tls`)
- `./ion_darts` file changed to direct to correct port.
- `blazing_sword` changed to point to correct port.


