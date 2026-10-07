# DanJa — установка на macOS

Подготовлена установка для Adobe After Effects 2026 на macOS. Проверка в реальном AE на Mac пока не проводилась.

1. Закрой After Effects.
2. Распакуй весь архив DanJa.
3. Открой Install-DanJa.command и подтверди установку клавишей Enter.
4. После установки запусти AE и открой Window → Extensions → DanJa.
5. Для записи пресетов включи Preferences → Scripting & Expressions → Allow Scripts to Write Files and Access Network.

Если Finder не запускает файл, открой Terminal, введи bash и пробел, перетащи Install-DanJa.command в окно Terminal и нажми Enter.
Если macOS показывает предупреждение безопасности, не отключай защиту системы; сообщи текст предупреждения для подготовки подходящего способа установки.

Панель устанавливается в ~/Library/Application Support/Adobe/CEP/extensions/com.danja.panel. Администраторские права не нужны.
Для неподписанной панели установщик записывает Adobe CEP PlayerDebugMode в com.adobe.CSXS.12.

Библиотека находится в папке DanJa внутри каталога пользователя Adobe ExtendScript Folder.userData. На macOS это обычно ~/Library/Application Support/DanJa.
Установщик не заменяет пользовательскую библиотеку. Предыдущая установленная панель сохраняется рядом в отдельной скрытой папке резервной копии.

Общие контроллеры создаются из переносимых FFX. В комплекте нет Windows DLL или EXE, от которых зависит работа панели. Превью встроены и не используют пути с исходного Windows-компьютера.

Необходимо проверить на Mac: открытие панели, кривые и Super Smooth, IN/OUT и изменение Offset, Fast Box Blur, сохранение пресета и рендер его превью, импорт/экспорт и удаление IN/OUT.

Версия остаётся 0.4.0. macOS предоставляется для тестирования; нативная проверка на Mac пока не завершена.
