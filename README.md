from aiogram import Bot, Dispatcher, types
from aiogram.utils import executor

TOKEN = "7558470396:AAHHA48hH_1BaIYm861dxHa6EQaQD3ZAUGg"  # Tokenni o'z botingdan ol

bot = Bot(token=TOKEN)
dp = Dispatcher(bot)

@dp.message_handler(commands=['start'])
async def start_command(message: types.Message):
    await message.reply("Salom! Men ishlayapman!")

if name == 'main':
    executor.start_polling(dp, skip_updates=True)
