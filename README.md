import requests

TOKEN = "8256443669:AAGiyoBvG1DxAK1TRUdR8yDiWD8P1huZX4U"
CHAT_ID = "1207611035"
TEXT = "Бот запущен! Всё работает."

r = requests.get(
    f"https://api.telegram.org/bot{TOKEN}/sendMessage",
    params={"chat_id": CHAT_ID, "text": TEXT}
)
print(r.text)   # чтобы видеть ответ Telegram
