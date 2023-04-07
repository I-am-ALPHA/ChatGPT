```
[✅] Created by using ChatGPT 3.5 turbo model.
     - Fork this Repo
     - Get OpenAI API key from https://platform.openai.com/account/api-keys and Replace it on key.json file.
     - Then Tap on Deploy button and Create new app. (for Heroku users)
     - Then go to Deploy tab and Connect to your GitHub.
     - After deployment is finished toggle worker button in Resources tab and Go to View logs.
     - Scan QR and Use your own ChatGPT WhatsApp bot.
```
<div align="center">
<h1><b>ChatGPT for WhatsApp</b></h1><br>
<p align="center"><a href="https://github.com/I-am-ALPHA"><img title="Author" src="https://img.shields.io/badge/Author-A L P H A-blue.svg?color=54aeff&style=for-the-badge&logo=github" /></p><br>
     
![image](https://telegra.ph/file/40ece39d93249caba8b1f.jpg)
 <br>

**A WhatsApp based 3ʳᵈ party OPEN-AI application that provide AI generated results with a real-time automated conversational experience. 👾**

**⚠️ Note: Make sure to replace your OpenAI API key in key.json before Deploy**

<a href="https://www.heroku.com/deploy/">
<img src="https://assets.strapi.io/uploads/Deploy_button_heroku_b1043fc67d.png" />
</a>

## Deploy on VPS.
 You need to Install git,ffmpeg,curl,nodejs,yarn with pm2 
   1. Install git ffmpeg curl 
      ```
       sudo apt -y update &&  sudo apt -y upgrade 
       sudo apt -y install git ffmpeg curl
      ```
   2. Install nodejs 
      ```
      sudo apt -y remove nodejs
      curl -fsSl https://deb.nodesource.com/setup_lts.x | sudo bash - && sudo apt -y install nodejs
      ```

   3. Install yarn
      ```
      curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - 
      echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
      sudo apt -y update && sudo apt -y install yarn
      ```

   4. Clone Repo and install required packages
      ```
      // Replace this link to your forked repo link in terminal
      git clone https://github.com/I-am-ALPHA/ChatGPT
      cd ChatGPT
      sudo yarn install --network-concurrency 1
      ```
  
   5. Start bot
      ```
      sudo yarn global add pm2 && pm2 start index.js --name ChatGPT && pm2 log ChatGPT
      ```
      
      ##
      
      If you are facing any problem, restart using this command
      ```
      pm2 restart ChatGPT
      ```


</div>
