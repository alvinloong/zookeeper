# ZooKeeper Overview

## [Getting Started](https://zookeeper.apache.org/doc/r3.6.1/zookeeperStarted.html)

### [Download](https://zookeeper.apache.org/doc/r3.6.1/zookeeperStarted.html#sc_Download)

```
sudo apt-get install openjdk-8-jdk
mkdir -p ~/soft/zookeeper/
tar -zxvf apache-zookeeper-3.6.1-bin.tar.gz -C ~/soft/zookeeper/
```

```
export ZOOKEEPER_HOME=$(pwd)
```

```
vi ~/.bashrc
```

```
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export ZOOKEEPER_HOME=/home/alvin/soft/zookeeper/apache-zookeeper-3.6.1-bin
export PATH=$ZOOKEEPER_HOME/bin:$PATH
```

```
source ~/.bashrc
```

### [Standalone Operation](https://zookeeper.apache.org/doc/r3.6.1/zookeeperStarted.html#sc_InstallingSingleMode)

```
cd $ZOOKEEPER_HOME
mkdir data
cp conf/zoo_sample.cfg conf/zoo.cfg
vi conf/zoo.cfg
```

```
dataDir=/home/alvin/soft/zookeeper/apache-zookeeper-3.6.1-bin/data
```

```
bin/zkServer.sh start
jps
```

