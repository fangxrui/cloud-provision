# ☁️Cloud-provision
## Intro  
 Provisioning a new server from a cloud provider at a particular region, that is initialized with a specified virtual machine image, using the [DigitalOcean api v2](https://docs.digitalocean.com/reference/api/api-reference/)
## How to run
`git clone` this repo

`cd` into the directory, then `npm install` to install dependencies

Set your token (generate by DigitalOcean)
```
# Mac/Linux
export MY_DOTOKEN="xxx"
# Windows
setx MY_DOTOKEN xxx
```

Run the node program by
`node index.js`

If everything is set correctly, you should see output like the following:

```
Your token is: xxxxxx
Calls remaining 4990
```

The provision() function in index.js includes a couple of steps for Listing regions, VM available images, creating droplet, getting droplet information, and testing whether the droplet is created or not.
