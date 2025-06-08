[Инструкция](https://pytorch.org/get-started/locally/) по установке. Код фреймворка на [GitHub](https://github.com/pytorch/pytorch). 

На Windows 11 может возникнуть ошибка `OSError: [WinError 126] The specified module could not be found. Error loading "fbgemm.dll" or one of its dependencies.`

Это может произойти по нескольким причинам: требуется Visual C++ Redistributable, не установлен видеодрайвер или отсутствует файл `libomp140.x86_64.dll` в `C:\Windows\System32\.` В последнем случае можно скачать или скопировать из другой системы файлы `libomp140.x86_64.dll` (желательно и debug версию `libomp140d.x86_64.dll`), скопировать в `System32`.
