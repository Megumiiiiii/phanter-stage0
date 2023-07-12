<div align="center">
 
# Phanter Protocol

</div>

<div align="center">

[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/Megumiiiiii)

 <img align="top" src="https://komarev.com/ghpvc/?username=Megumiiiiii&color=ff69b4&style=plastic&label=Visitors" height='35'/>

</div>

#

<div align="center">
  
## ${\color{violet} COPAS \space SERTAIN \space SUMBER \space SU}$

### ${\color{violet} DIKIRA \space BIKIN \space GINIAN \space GAK \space PERLU \space USAHA \space APA}$ 

</div>

## Official Links
- [How To](https://blog.pantherprotocol.io/testnet-stage0-live/#how-to-test)
- [Discord](https://discord.gg/x3evTkDbch)
- [Twitter](https://twitter.com/zkpanther)


### Install Docker (Jika belum)

```yml
sudo apt update; sudo apt upgrade -y
```

```yml
sudo apt-get update && sudo apt install jq git && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin && sudo apt-get install docker-compose-plugin
```

### Atur keperluan

```yml
git clone https://github.com/Megumiiiiii/phanter-stage0.git
cd ~/phanter-stage0
```

#### Edit .env

```yml
cp .env.sample .env
```


```yml
nano .env
```

- isi yang kosong, `RPC_URL` isi dengan HTTPS Polygon Mumbai dari Alchemy -> [Alchemy](https://dashboard.alchemy.com/)
- ![alchemy](https://github.com/Megumiiiiii/phanter-stage0/assets/98658943/87f66461-5f75-45b0-b6d9-c5eed4914829)
- `PRIVATE_KEY` isi dengan privkey dari Metamask **WALLET BARU** atau **WALLET TESTNET**, dan ambil faucet Matic testnet -> [DISINI](https://mumbaifaucet.com/)
- ![Aenv](https://github.com/Megumiiiiii/phanter-stage0/assets/98658943/d7efb5d3-2e3b-467e-a986-3b46ddc4a888)

### Memulai Node

#### Pull

```yml
docker pull pantherprotocol/miner-client
```

## RUN !1!1!1

```yml
docker run -d \
--restart always \
--pull always \
--name panther \
--env-file .env \
pantherprotocol/miner-client
```

### Cek logs

```yml
docker logs -f panther
```

### ⚠️ Jika ingin menghapus node ⚠️

```yml
docker stop panther; docker rm panther
docker rmi pantherprotocol/miner-client
```

#

<div id="header" align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMzNmZTIxZmE3ZmY3MzRiMDcwNDJhYTQ5ZmNlY2YxMWE1OWIyYmVkNSZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/mVBlqOD4ra9jQiI3cC/giphy.gif" height="125" width="420"/>
</div>
