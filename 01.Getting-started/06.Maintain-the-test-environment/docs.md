---
title: Maintain the demo environment
taxonomy:
    category: docs
---

You can find some steps for maintaining your demo environment below.


## Stop the Mender services

When you are done testing Mender, simply press **Ctrl-C** in the terminal
you started Mender in, where the log output is shown. Stopping all the
services may take about a minute.

The Mender demo environment can be started by running the `up` script again.


## Reset login credentials

If you just lost the login credentials, you can run the `reset-user` script in the `integration` directory.


## Clean up the environment

!! You will lose all state data in your Mender demo environment by running the commands below, which includes devices you have authorized, software uploaded, logs, deployment reports and any other changes you have made.

If you want to remove all state in your Mender demo environment and start clean,
run the following commands in the `integration` directory:

```bash
./stop
```

```bash
./reset
```

```bash
./up
```
