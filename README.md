# Hadoop

## Puertos

| Nombre  | Puerto Anfritión | Puerto Invitado|
| ------------- | ------------- | ------------- | 
| ssh  | 2222  | 22 |

## Acceso

```
ssh cloudera@localhost -p 2222
```

## Instalación

### Python

```
cd
wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
chmod a+x Miniconda2-latest-Linux-x86_64.sh
./Miniconda2-latest-Linux-x86_64.sh
```

### Python 3
```
conda create -n py36 python=3.6

source activate py36
source deactivate
```

### Clave ssh

```
cd
ssh-keygen -t rsa -b 4096 -C "dvillaj@gmail.com"
cat .ssh/id_rsa.pub
```

### Git
```
git config --global user.name "Daniel Villanueva"
git config --global user.email "dvillaj@gmail.com"
```

### Kafka
```
cd
wget http://apache.rediris.es/kafka/1.0.0/kafka_2.11-1.0.0.tgz
tar -xzf kafka_2.11-1.0.0.tgz
cd cd kafka_2.11-1.0.0

bin/kafka-server-start.sh config/server.properties &

```
