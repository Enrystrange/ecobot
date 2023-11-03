import discord
from discord.ext import commands
import random

intents = discord.Intents.default()
intents.message_content = True

bot = commands.Bot(command_prefix='$', intents=intents)

@bot.event
async def on_ready():
    print("Hai fatto l\'accesso come {bot.user}")
@bot.command()
async def fazzoletto(ctx):
    await ctx.send(f' 10 settimane')
@bot.command()
async def plastica(ctx):
    await ctx.send(f'ci vogliono 30 anni')
@bot.command()
async def vetro(ctx):
    await ctx.send(f'ci vogliono 4000 anni')
@bot.command()
async def bioplastica(ctx):
    await ctx.send(f'ci vogliono 20 giorni')
@bot.command()
async def sigarette(ctx):
    await ctx.send(f'ci vogliono 8 anni')
bot.run("MTE2Nzc2MTc3MzE4OTkzMTExOA.GxKx50.I5uFztWPTZtV_c6lt2EOGBbxpY5i31TjEMmgP8")
