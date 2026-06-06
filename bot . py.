import asyncio
import os
from telegram import Bot
from datetime import datetime

BOT_TOKEN = os.environ.get("BOT_TOKEN")
CHANNEL_ID = os.environ.get("CHANNEL_ID")
MESSAGE = "اللهم صل وسلم على رسول الله ﷺ"

async def send_salawat():
    bot = Bot(token=BOT_TOKEN)
    print("✅ البوت بدأ يعمل...")
    while True:
        try:
            await bot.send_message(chat_id=CHANNEL_ID, text=MESSAGE)
            print(f"✅ تم الإرسال: {datetime.now().strftime('%Y-%m-%d %H:%M:%S')}")
        except Exception as e:
            print(f"❌ خطأ: {e}")
        await asyncio.sleep(3600)

if __name__ == "__main__":
    asyncio.run(send_salawat())
