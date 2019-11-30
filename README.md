# Godfather-Test-Bot
const {Client, RichEmbed} = require('discord.js');
const bot = new Client();

const token = 'NjUwMDc3Njc5Mzc0MTcyMTYw.XeH3sg.c9Dzh7_NFNI48hvtVUuzfuwS4fs';

const PREFIX = '!';


bot.on('ready', () => {
    console.log('This bot is active!');
})

bot.on('message', message => {
    let args = message.content.substring(PREFIX.length).split(" ");
    

    switch (args[0]) { 
        case 'help':
            const Embed = new RichEmbed()
            .setTitle("Helper Embed")
            .setColor(0xFF0000)
            .setDescription("Make sure to use the !help to get access to the commands");

            message.author.send(Embed);
        break;
    }


});

            
                        
bot.login(NjUwMDc3Njc5Mzc0MTcyMTYw.XeH3sg.c9Dzh7_NFNI48hvtVUuzfuwS4fs);
