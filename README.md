# gNB_Conf_Files
Conf files to run Radio and SDR

## To run Radio
- [LiteOn](./RADIO/LiteOn/)
    -   https://github.com/NgKore47/Liteon-ngKore_E?tab=readme-ov-file#14-run-oai-gnb
- [Picocom](./RADIO/Picocom/)

## SDR
- [USRP_B210](./SDR_USRP/USRP_B210/gnb.sa.band78.fr1.106PRB.usrpb210.conf)

```bash
sudo ./nr-softmodem -O ../../../targets/PROJECTS/GENERIC-NR-5GC/CONF/gnb.sa.band78.fr1.106PRB.usrpb210.conf --sa -E --continuous-tx
```

- [USRP_N310](./SDR_USRP/USRP_N310/)

#### For 1T1R:
```bash
sudo ./nr-softmodem -O Gabriel_N310_1T1R.conf --sa --usrp-tx-thread-config 1
```

#### For 2T2R
```bash
sudo ./nr-softmodem -O ../../../targets/PROJECTS/GENERIC-NR-5GC/CONF/gnb.sa.band78.fr1.106PRB.2x2.usrpn300.conf --sa --usrp-tx-thread-config 1 -E --continuous-tx
```

- [USRP_X410](./SDR_USRP/USRP_X410/1T1R_Config/gnb.sa.band78.fr1.106PRB.usrpx310.conf)

```bash
sudo ./nr-softmodem -O usrp_x410_1t1r.conf --sa --usrp-tx-thread-config 1
```