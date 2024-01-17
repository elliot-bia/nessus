<div align="center">

# Nessus docker crack version

<br>

<a href="https://twitter.com/Elliot58616851" target="_blank"><img src="https://img.shields.io/twitter/follow/Elliot58616851?style=social"> </a>

<div>
    <img alt="platform" src="https://img.shields.io/badge/platform-Docker%20%7C%20DockerFile-blueviolet">
</div>
<div>
    <img alt="license" src="https://img.shields.io/github/license/elliot-bia/nessus?logo=1">
    <img alt="stars" src="https://img.shields.io/github/stars/elliot-bia/nessus?style=social">
</div>

<br>

[🇨🇳简体中文](./README-cn.md) | [🇺🇸English](./README.md) | [🇩🇪Deutsch](./README-de.md)

This project is only for non-profit learning research. Do not use it for illegal purposes. If there is any infringement, please contact it in time to delete it.
</div>

# Usage
`docker run -itd --name=ramisec_nessus -p 8834:8834 ramisec/nessus`  ~~(497MB Only!!!)~~ (It takes 885MB now because of adding openjdk8)

That's right, easy like that! But it need update the plugins with the following command. 🤣  

# Update
`docker exec -it ramisec_nessus /nessus/update.sh "UPDATE_URL_YOU_GOT"`  
The **UPDATE_URL_YOU_GOT** you need to apply in nessus [website](https://tenable.com/products/nessus/nessus-essentials) to get **an activation-code**, and generate it in this [website](https://plugins.nessus.org/v2/offline.php)  
For example:

<img width="544" alt="image" src="https://github.com/elliot-bia/nessus/assets/40572216/0a821a76-060c-4b51-a1a4-f95bd56e2556">  

Any stings like `aaaaaa11b2222cc33d44e5f6666a777b8cc99912` would be available, but remeber must not be the same :)  

And you will get the **UPDATE_URL_YOU_GOT**  

<img width="540" alt="image" src="https://github.com/elliot-bia/nessus/assets/40572216/486988b6-352e-4d8e-9910-1308c50bc053">  

__Alert__  
If you CAN NOT update successful, please CHECK the network connection!

# Migration

If you need to migrate from old versions to new, use the following command

```bash
# Crate dir
mkdir ~/nessus_data
# Stop container
docker stop ramisec_nessus
# copy data
docker cp ramisec_nessus:/opt/nessus/var/nessus/ ~/nessus_data
# delete old container
docker rm ramisec_nessus
# run new container
docker run -itd --name=ramisec_nessus -v ~/nessus_data/nessus/:/opt/nessus/var/nessus/ -p 8834:8834 ramisec/nessus
# update plugins
docker exec -it ramisec_nessus /bin/bash /nessus/update.sh
```

# Account & Password

account: `admin`

Password: Easter Egg! Check the change version  
Let you explore the function, if you solved the password, Keep It Secret😉

# Readme

This crack was originally used, and I didn't plan to make it public  
But when I used the FAHAI cracked version of AWVS yesterday, I saw such a sentence:  
`Thank's Fahai && Open Source ENTHUSIAST`  
 <img src="https://user-images.githubusercontent.com/40572216/174698816-440d4969-f9d6-4c7d-982c-9af9c4a3e875.png" width = "400" height = "200" alt="图片名称" align=center />

So I was thinking, I used so many open source projects, how many contributions did I make?  
I simply disclose this project, which can also be considered a little contribution to the Internet security  
If there is no accident, it will continue to be updated, after all, I also need to use  
~~Don't get the automatic update plug -in version, use it first!~~  
I had release auto-update version, check Update log!

The Original Intention of the Project is in the Spirit of Open Source  
We can do a little thing for open source, for the world!  

# Update log

## v5 20231218

- Fix Crack fail situation

- Add openjdk-8-jdk

## v4 20230523

- Fix Timezone error

- Add scan data migration

- Change password

  **tips：npaobi/lsspva-iph/ulzzbz**

  **Alea iacta est，Destiny reveals that your lucky number is 7.**

## v3 20220722

__Big update：auto-update plugins version has release！__

usage： `docker run -itd --name=ramisec_nessus -p 8834:8834 ramisec/nessus`  
The container had no plugins, it need to update by following command:  
`docker exec -it ramisec_nessus /bin/bash /nessus/update.sh`  
and it can be update again next time by the same command ！



## v2 20220621

Update the latest version of 20220620, and use 2 versions of NESSUS/JESSUSLITE  
The former has been cracked and compiled the plug -in.  
The latter needs to wait a few minutes to compile the plug -in  
password:  
`U2FSDGVKX19WZV+Qoe8awvyjwxDPSNSIC1X4AMNA4+3RO8ml/3Hz+MS/OR3DHCWXKS0WHFVOH1Q/yntvdxnahg ==`  

__TIPS__: gitHub/elliot-bia


> ~~# Old Usage~~
> ~~`docker run -itd -p 8834:8834 ramisec/nessus`   (4.73GB)~~
> ~~ or~~  
> ~~`docker run -itd -p 8834:8834 ramisec/nessuslite` (3.55GB)~~ 
> ~~The former does not require compilation and is suitable for low-performance high-bandwidth machines~~  
> ~~The latter requires compilation and is suitable for high-performance low-bandwidth machines~~  
> ~~What? high-performance and high-bandwidth machines? Never mind, just use it! have fun!~~

In fact, there is another EASY way to solved the encryption, try and find it!😆

# Thanks note
Some English text translated by [Aholicknight](https://github.com/Aholicknight)

thanks a lot! 

# donate
If you like this project, you can be a sponsor!  

[Pay Me via PayPal](https://www.paypal.com/paypalme/pay2rami)