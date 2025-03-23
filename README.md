import keyboard  # для отслеживания нажатий клавиш
import webbrowser  # для открытия веб-страниц

# Функция, которая открывает YouTube
def open_youtube():
    webbrowser.open("https://www.youtube.com")

# Назначаем функцию на нажатие клавиши "ю"
keyboard.add_hotkey('ю', open_youtube)

# Бесконечный цикл, чтобы программа не завершалась
print("Бот запущен. Нажмите 'ю', чтобы открыть YouTube.")
keyboard.wait('esc')  # Ожидание нажатия клавиши Esc для выхода
