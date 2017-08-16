Deploy in the following order to prevent race conditions:

1. elasticsearch
2. mariadb
3. kibiter
4. kibana
5. mordred

Adjust the mordred configuration files in ./conf.  For more details see: [https://github.com/grimoirelab/mordred/tree/master/docker](https://github.com/grimoirelab/mordred/tree/master/docker)