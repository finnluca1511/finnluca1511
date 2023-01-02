python3 -m pip install -U discord.py[voice] 

import os
import discord

import os
import discord

client = discord.Client() 

@client.event
async def on_ready():
    print(f'Logged in as {client.user}') 
    
    @client.event
async def on_message(message):
    if message.author == client.user:
        return

    if message.content == 'Hi bot':
        await message.channel.send('Hello human!')
        
        TOKEN = os.getenv('DISCORD_TOKEN')
        
        client.run(TOKEN)
        
        DISCORD_TOKEN=YOUR_TOKEN python3 YOUR_BOT_FILE.py
