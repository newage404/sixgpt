# **Sixgpt Miner**

Guide on how to run sixgpt Miner

# Requirement

(1) install docker on your machine.

(2) Make sure you already log in with your wallet on [sixgpt](https://sixgpt.xyz/) (burner recommended)

(3) Fund your wallet with at least 0.1 $VANA, request Vana [faucet](https://faucet.vana.org/satori)


# Update Package list
```bash
sudo apt update 
sudo apt upgrade -y
```

# Kickstart Miner
Clone the repository 

```bash
git clone https://github.com/sixgpt/miner.git
cd miner
```

**Set the following Environment variable**

**_note: replace the <your_private_key> with your wallet PK_** 

```bash
export VANA_PRIVATE_KEY=<your_private_key>
export VANA_NETWORK=satori
```

# Run the miner

```bash
docker compose up
```

# Check Miner status 
```bash
sudo docker logs ollama -f -n 50
```
