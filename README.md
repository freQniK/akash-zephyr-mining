# akash-zephyr-mining
Mining Zephyr Protocol on Akash to Herominers

## Edit fields

The first field you *can* edit is the docker image of xmrig:

### Docker Image
```shell
image: 4nroi7q8/xmrig:20231123
```

Now, you will just have to take my word for this as it isn't verifiable, but I have built this image from source with a **ZERO** dev fee. You are happy to build your own docker image or use someone elses.

### Zephyr Wallet Address

Edit the following with our wallet:

```shell
- WALLET=
```

### Worker/Pass

You can change the name of your worker by editing the following:

```shell
- WORKER=akash
#All worker names have the provider domain as suffix, example akash-provider.akash.world
- PASS=akash
```

### Number of CPUs

Change the following parameter to determine how may vCPUs you will be using on Akash

```shell
cpu:
  units: 32
  #Min 0.01 / Max 256 cpu.units
```

## Hindsight
Honestly, I have not received great Hashrate on Akash and am a little disappointed. The very first deployment I was getting 10Kh/s and it dropped off within the hour to around 2Kh/s. The parameters was 32 vCPUs and cost was around 27 **AKT** per month. 

It is best to try a lot of deployments to get a better gauge of what the nodes can handle. You may experience with some of the nodes that xmrig does not run. If this is the case close the deployment and try another provider. 



