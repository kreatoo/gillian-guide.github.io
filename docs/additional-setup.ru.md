title: Второстепенная настройка
description: Второстепення настройка для вашей установки GTA IV - после выполнения оптимизации или установки готового архива

# Второстепенная настройка
Независимо от того, пришли ли вы сюда после использования [готового архива](drag-and-drop-archive.md) или после [оптимизации](optimization.md), нам все ещё необходимо выполнить второстепенную настройку для достижения наилучшего опыта игры.

## Параметры запуска
???+ note "Как выставить параметры запуска?"
    Есть несколько способов:
    
    1. Зайдите в меню Свойства игры в :material-steam:Steam и выставите их там;
    2. Создайте в папке с игрой :material-file-cog:`commandline.txt` и отредактируйте его ==(этого сделать нельзя на Complete Edition)==;
    3. Создайте ярлык для игры и добавьте параметры после пути к ярлыку.

    Мы ограничимся первыми двумя.

Единственные опции, что вы должны выставить: `-norestrictions -nomemrestrict`.

??? warning "При использовании DXVK или готового архива..."
    * Добавьте `-windowed` для использования безграничного полноэкранного режима для большей стабильности. Убедитесь, что `BorderlessWindowed` включён в :material-file-cog:`ZolikaPatch.ini` и/или :material-file-cog:`GTAIV.EFLC.FusionFix.ini`.
    * Если в настройках графики игра не показывает нужного объема VRAM (например, 512 МБ), добавьте `-availablevidmem` с значением видеопамяти вашего ГП с `.0` в конце - до `3072.0`.
    * Если игра не позволяет использовать правильное разрешение/частоту обновления, добавьте `-width`, `-height` и `-refreshrate` с "родными" значениями вашего монитора.
    * Вы также можете добавить `-managed` для увеличенной производительности, но ваша игра может чаще вылетать, особенно с опцией `nomemrestrict`.

!!! danger "Но в других гайдах используют больше настроек!"
    ^^Не используйте их^^. Может быть, они и помогли бы в 2009 году, когда обычные пользовательские ПК не могли справиться с прекэшированием и прочим, но сейчас эти опции только ухудшают ситуацию или выступают в роли чистого плацебо. Если ваш [мод](extras/mods.md) требует какую-то настройку - добавляйте.

??? abstract "Полный список параметров запуска"
    Эти опции можно использовать для настройки и отладки. Список взят из [PCGW](https://www.pcgamingwiki.com/wiki/Grand_Theft_Auto_IV#Launch_options)

    | Настройка | Описание | 
    | --------: | :------- |
    | -help | Список доступных команд. |
    | -adapter | Используется указанный адаптер экрана. |
    | -autoconfig | Автоматически настраивает графические параметры в зависимости от характеристик компьютера. |
    | -availablevidmem | Устанавливает объем доступной физической видеопамяти. |
    | -benchmark | Запускает игру в режиме Benchmark и затем завершает ее. |
    | -detailquality | Устанавливает глубину детализации игры (0-99). |
    | -disableimposters | Отключает рендеринг ненастоящего траффика в далеке. |
    | -forcehighqualitymirrors | ? |
    | -forcer2vb | Принудительный рендеринг в Vertex Buffer. |
    | -frameLimit | Устанавливает настройку для V-Sync. |
    | -framelockinwindow | Заставляет framelock работать даже в окне. |
    | -fullscreen | Заставляет полноэкранный режим. |
    | -fullspecaudio | Принудительное использование высоко-качественного звука. |
    | -gpucount | Позволяет вручную установить количество GPU, если запрос не выполняется. |
    | -height | Устанавливает вертикальное разрешение. |
    | -managed | Использует управляемые ресурсы времени выполнения D3D. |
    | -memrestrict | Ограничивает объем доступной памяти, которую может использовать игра. |
    | -minspecaudio | Принудительное использование низко-качественного звука. |
    | -no_3GB | Отключает поддержку памяти 3 ГБ в 32-разрядных ОС, в которых установлено, что игры и приложения могут использовать такой объем памяти. |
    | -noBlockOnLostFocus | Запрещает игре блокировать обновление окна при потере фокуса.  |
    | -noprecache | Отключает предварительное кэширование ресурсов. |
    | -nomemrestrict | Отключает ограничение памяти. |
    | -nominimize | Отключает возможность восстановления игры из режима минимизации и изменения разрешения (уменьшает занимаемую системную память). |
    | -norestrictions | Отключает ограничения на настройки графики. |
    | -noswapdelay | Отключает задержку перед Present (отключает исправление hard present stalls). |
    | -notimefix | Отключает Time Fix. |
    | -novblank | Отключение вертикального бланкирования для V-Sync. |
    | -percentvidmem | Процент видеопамяти, который должен быть доступен для игры. |
    | -refreshrate | Устанавливает частоту обновления (установленные значения должны поддерживаться используемым монитором). |
    | -reserve | Устанавливает объем памяти, который будет использоваться другими программами. |
    | -reservedApp | Устанавливает объем памяти, который должен оставаться доступным в пространстве приложения. |
    | -renderquality | Настраивает анизотропную фильтрацию (0-4). |
    | -safemode | Устанавливает минимально возможные настройки графики игры. |
    | -shadowdensity | Настраивает ночные тени (0-16). |
    | -shadowquality | Устанавливает качество теней (0-4). |
    | -stereo | Включает поддержку стереозвука. |
    | -texturequality | Устанавливает качество текстур игры (0-2). |
    | -unmanaged | Использует ресурсы, управляемые приложением. |
    | -usedirectinput | Позволяет использовать поддержку DirectInput наряду с поддержкой XInput. |
    | -viewdistance | Устанавливает расстояние обзора игры (0-99). |
    | -windowed | Устанавливает оконный режим. |
    | -width | Устанавливает разрешение по горизонтали. |

## Оптимальные настройки графики
![Настройки GTA IV](assets/gta4settings.jpg){: style="height:25%;width:25%"; align=right}
!!! note ""
    Эти настройки оптимальны для большинства пользователей. Если ваш компьютер слабее - можете их понизить. Если ваш компьютер мощнее - можете их повышать, но не вините меня в возникших проблемах.

??? info "Консольные настройки"
    Эти настройки были установлены на консольных версиях игры, и игра наиболее оптимизирована для них. Они включены ради полноценного списка.
| Настройка | Оптимальная настройка | Консольная настройка | Описание | 
| :-------: | :-------------------: | :------------------: | :------: |
| Видеорежим | Ваше сообственное разрешение (максимальное, обычно) | 1280x720 на Xbox 360; 1152x640 на PlayStation 3; оба работали с частотой 20-30 FPS | Эта настройка контролирует разрешение вашего монитора или, если установлен параметр запуска `-windowed`, размер игрового окна. |
| Соотношение сторон | Авто | Авто | Этот параметр определяет соотношение сторон экрана относительно разрешения вашего монитора. |
| Качество текстур | Высокое | Среднее | Эта настройка регулирует разрешение всех текстур. |
| Разрешение отражений | Очень высокое | Среднее | Эта настройка регулирует разрешение отражений (кроме отражений в воде). |
| Качество воды | Среднее | Среднее | Эта настройка регулирует плотность и интенсивность волн в воде и образцах воды, а также разрешение отражений в воде. Рекомендуется использовать Среднее, так как оно менее экстремально и более реалистично. [Shader Fixes](essential-modding/shader-fixes.md) позволяет сохранить максимальное (1024x1024) разрешение отражений при более низких параметрах. |
| Качество теней | Высокое | Среднее | Этот параметр регулирует разрешение и расстояние рендеринга теней. Среднее и низкое качество полагаются на статические тени больше, чем Высокое. Очень высокое  потребляет ~20 FPS. |
| Улучшенные ночные тени | Среднее или Очень высокое | Откл | Этот параметр определяет, сколько локальных огней (например, фар автомобиля) могут отбрасывать тени. Каждый уровень качества добавляет 4 дополнительные карты теней. Эта настройка не влияет на разрешение динамических теней. [FusionFix](essential-modding/fusionfix.md) позволяет улучшить эту настройку, добавив динамические тени к большинству объектов. И [FusionFix](essential-modding/fusionfix.md), и [Shader Fixes](essential-modding/shader-fixes.md) исправляют артефакты, возникающие при использовании этой настройки. |
| Качество фильтрации текстур | Анизотропная 16x | Трилинейная | Эта настройка управляет анизотропной фильтрацией. |
| Дистанция обзора | Между 21 и 70 | 21 | Эта настройка контролирует основное расстояние рендеринга LOD для таких объектов, как здания и транспорт. Также контролирует расстояние рендеринга пропов. Установка значения выше 70 приводит к нестабильности и артефактам, а также негативно сказывается на FPS. |
| Глубина детализации | Между 10 и 70 | 10 | Этот параметр управляет расстоянием вторичного рендеринга LOD для деталей в пропах. Установка значения выше 70 может привести к нестабильности и появлению артефактов. |
| Транспортный поток | По предпочтению - желательно менее 90 | 33 | Этот параметр регулирует плотность движения. Слишком высокое значение может сделать вождение слишком надоедливым, особенно с нестабильным ИИ трафика, который может иногда создавать случайные заграждения даже на прямых дорогах и мостах. |
| Глубина поля наблюдения | Откл | Откл | Эта настройка регулирует глубину резкости и размытие в движении - однако, она также вызывает проблемы с размытой картинкой на ПК и эффектами, которые просто не масштабируются по разрешению - используйте [Shader Fixes](essential-modding/shader-fixes.md) для исправления проблемы. Можно быстро переключать кнопкой ++p++. |
| FXAA | Вкл | - | Эта настройка управляет FXAA (простой метод сглаживания) - используйте [FusionFix](essential-modding/fusionfix.md) для её появления, или [Shader Fixes](essential-modding/shader-fixes.md) чтобы всегда иметь FXAA. |
| Вертикальная синхронизация | Откл | Вкл |  Эта настройка управляет вертикальной синхронизацией. Мы будем использовать ту, которая поставляется [DXVK](optimization.md), поскольку она имеет гораздо лучшую синхронизацию кадров. |

??? question "Что такое :material-file-cog:`stream.ini`?"
    В других руководствах часто используют :material-file-cog:`stream.ini` и меняют в нем значения с `2048000` на `4096000`. По [наблюдениям пользователей PCGW](https://www.pcgamingwiki.com/w/index.php?title=Topic:X1jmh4mc3t6mv3hv&topic_showPostId=xb5gbd4mggke2ets#flow-post-xb5gbd4mggke2ets), а также моими собственным - это не дает никакого эффекта и, скорее всего, является плацебо.

Если вы хотели лишь улучшить производительность то на этом можно и остановиться, однако я бы посоветовал добраться до установке важных модов для получения лучшего опыта игры.

[:material-page-first:Предыдущая страница <br>Оптимизация</br>](optimization.md){ .md-button } [Следующая страница:material-page-last: <br>Даунгрейд</br>](downgrading.md){ .md-button .md-button--primary }