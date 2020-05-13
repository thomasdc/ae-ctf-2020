# Prerequisites
- Make sure you have Docker installed
- Clone this repo

# Hosting Juice Shop locally
Run the following command in the root of the repo you just cloned.

## Windows
```
docker run -d -e "NODE_ENV=ae-ctf-2020" -v %cd%\config:/juice-shop/config -p 3000:3000 --name juice-shop bkimminich/juice-shop
```

Allow Docker for Windows to access your C: drive if needed.

## Linux
```
docker run -d -e "NODE_ENV=ae-ctf-2020" -v $(pwd)/config:/juice-shop/config -p 3000:3000 --name juice-shop bkimminich/juice-shop
```

# Tips
You can view the logs of your local Juice Shop container like this:
```
docker logs juice-shop -f
```
