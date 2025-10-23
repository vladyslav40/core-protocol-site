<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rivestor // CORE PROTOCOL</title>
    <style>
        /* ====================
           1. ОБЩИЕ СТИЛИ
           ==================== */
        body {
            font-family: 'Consolas', 'Courier New', monospace;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #000000; /* Начальный черный фон */
            color: #ffffff;
            text-align: center;
            overflow: hidden;
            position: relative;
            transition: background-color 0.1s; /* Для резкого перехода */
        }

        /* Общий контейнер для слов в первой фазе */
        .intro-words {
            position: absolute;
            z-index: 100;
        }

        /* ====================
           2. ФАЗА 1: НАБОР И УДАЛЕНИЕ (TYPE/DELETE EFFECT)
           ==================== */
        .word-container {
            font-size: 5.5rem; /* Очень крупный шрифт */
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            display: flex; /* Для курсора */
            justify-content: center;
            align-items: center;
            height: 100vh;
            color: #ffffff;
        }

        .typing-text {
            overflow: hidden;
            white-space: nowrap;
            display: inline-block;
            opacity: 0; /* Скрыто до начала анимации */
        }
        
        /* Мигающий курсор */
        .cursor {
            border-right: 0.15em solid #ffffff; 
            animation: blink-caret 0.75s step-end infinite;
            height: 1em;
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: white; }
        }

        /* ====================
           3. ФАЗА 1.5: 3D-ВСПЫШКА (СЛОВО FREEDOM)
           ==================== */
        .final-word {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 0; /* Изначально скрыто */
            font-weight: 900;
            text-transform: uppercase;
            color: #ffffff;
            z-index: 200;
            opacity: 0;
        }

        @keyframes finalExplosion {
            0% { 
                font-size: 5rem; 
                opacity: 1; 
                filter: blur(0px); 
                transform: translate(-50%, -50%) perspective(100px) translateZ(0);
            }
            80% { 
                font-size: 200vw; /* ОГРОМНЫЙ РАЗМЕР */
                opacity: 1; 
                filter: blur(5px); 
                transform: translate(-50%, -50%) perspective(100px) translateZ(100px); /* 3D-эффект */
            }
            100% { 
                font-size: 200vw; 
                opacity: 0; 
                filter: blur(10px); 
                background-color: #ffffff; 
            }
        }
        
        .final-word.explode {
            animation: finalExplosion 1.0s ease-in forwards;
            animation-delay: 0.2s;
        }


        /* ====================
           4. ФАЗА 2: БЕЛЫЙ ЭКРАН / КОНТЕНТ
           ==================== */
        
        body.white-phase {
            background-color: #ffffff;
            color: #000000;
        }

        .main-content {
            opacity: 0;
            transition: opacity 1.5s ease-in-out 0.1s; 
            max-width: 800px;
            padding: 40px 20px;
            margin-top: 200px; /* Сдвиг текста вниз */
            position: relative; 
            z-index: 20;
                   
        }
        
        .main-content.active {
            opacity: 1;
        }

        /* ЛОГОТИП (750px) */
        .logo-wrapper {
            width: 750px; 
            height: 750px;
    
            position: absolute;
            top: -20%; /* Сдвиг логотипа вверх */
            left: 50%; 
            transform: translate(-50%, -50%) scale(0.6); 
    
            z-index: 1; 
    
            opacity: 0;
            /* Убрана задержка, чтобы оно появлялось одновременно с main-content */
            transition: opacity 1.5s ease-out, transform 1.5s ease-out; 
            pointer-events: none;
        }

        .logo-wrapper.active {
            opacity: 1;
            transform: translate(-50%, -50%) scale(1); 
        }
        
        .logo {
            width: 100%;
            height: 100%;
            background-image: url('RivestorLogo.png');
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
        }

        /* ТЕКСТ (ВАШ ОРИГИНАЛ) */
        .headline {
            font-size: 4.5rem;
            font-weight: 700;
            line-height: 1.1;
            margin-bottom: 30px;
            text-transform: uppercase;
        }

        .subtext {
            font-size: 1.25rem;
            color: #444;
            margin-bottom: 50px;
        }

        /* КНОПКА (СВЕЧЕНИЕ И ЗАКРУГЛЕНИЕ) */
        .cta-button {
            padding: 20px 40px;
            font-size: 1.2rem;
            font-weight: 700;
            color: #ffffff;
            background-color: #000000;
            border: none;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 2px;
            
            /* НОВЫЕ СТИЛИ ДЛЯ КНОПКИ */
            border-radius: 8px; /* ЗАКРУГЛЕННЫЕ УГЛЫ */
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.4); /* ЛЕГКОЕ СВЕЧЕНИЕ */

            transition: background-color 0.1s, transform 0.1s, box-shadow 0.3s;
        }

        .cta-button:hover {
            background-color: #333333;
            transform: scale(0.98);
            box-shadow: 0 0 25px rgba(0, 0, 0, 0.7); /* Свечение при наведении */
        }
        /* 1. Новая анимация затухания */
        @keyframes fadeToTransparent {
            0% { opacity: 0; }      /* Начинаем с невидимости */
            5% { opacity: 0.1; }    /* Быстро доходим до 50% */
            100% { opacity: 0.05; }  /* Плавно затухаем до 10% */
        }
        /* ====================
   4.5. PNG-РАМКА (НОВЫЙ БЛОК)
   ==================== */
        .overlay-frame {
            position: fixed; /* Фиксируем на экране */
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
    
    /* УКАЗЫВАЕТ НА ВАШ ФАЙЛ background1.png */
            background-image: url('background3.png');
            background-size: cover; 
            background-repeat: no-repeat;
            background-position: center;
    
            z-index: 10; /* <-- Слой рамки (между текстом и лого) */
            pointer-events: none; /* Позволяет кликать сквозь рамку по кнопке */
            opacity: 0; 
            transition: opacity 1.5s ease-in-out 0.1s;
        }

        .overlay-frame.active {
            animation: fadeToTransparent 3s ease-out forwards;
        }
        /* ==================== */

        /* ====================
           5. МЕДИА-ЗАПРОСЫ (АДАПТИВНОСТЬ)
           ==================== */
        @media (max-width: 768px) {
            .word-container { font-size: 3rem; }
            
            .headline { font-size: 2.5rem; margin-bottom: 20px;}
            .subtext { font-size: 1rem; margin-bottom: 30px; }
            
            .main-content { 
                padding: 20px;
                margin-top: 50px; /* Меньший сдвиг вниз для мобильных */
            }

            /* АДАПТАЦИЯ ЛОГО ДЛЯ МОБИЛЬНЫХ */
            .logo-wrapper { 
                width: 400px; 
                height: 400px;
                top: 25%; /* Сдвиг логотипа выше на маленьких экранах */
            }
            .final-word { font-size: 3.5rem; }
            .cta-button { padding: 15px 30px; font-size: 1rem; }
        }
    </style>
</head>
<body>
    <div class="overlay-frame" id="overlay-frame"></div>
    <div class="intro-words" id="intro-words">
        <div class="word-container">
            <span class="typing-text" id="typing-text-target"></span>
            <span class="cursor" id="cursor-target"></span>
        </div>
        <div class="final-word" id="final-word">FREEDOM</div>
    </div>
    
    <div class="main-content" id="main-content">
        
        <div class="logo-wrapper" id="logo-wrapper">
            <div class="logo"></div>
        </div>
        
        <h1 class="headline">
            YOUR FUND, YOUR FREEDOM
        </h1>
        
        <p class="subtext">
            Rivestor is building a platform to create, manage, and grow decentralized funds powered by AI and on-chain transparency. Enter your email below to get exclusive updates and early access to the platform.
        </p>

        <button type="button" class="cta-button" onclick="window.location.href='ВАША_ССЫЛКА_СЮДА'">
            INITIATE ACCESS
        </button>
    </div>
    
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const body = document.body;
            const typingTarget = document.getElementById('typing-text-target');
            const cursorTarget = document.getElementById('cursor-target');
            const finalWord = document.getElementById('final-word');
            const introContainer = document.getElementById('intro-words');
            const mainContent = document.getElementById('main-content');
            const logo = document.getElementById('logo-wrapper');

            const concepts = [
                "AUTONOMY",
                "YIELD",
            ];
            const finalConcept = "FREEDOM";

            let conceptIndex = 0;
            let charIndex = 0;
            let isDeleting = false;

            // Функция Набора и Удаления
            function typeWriter() {
                const currentText = concepts[conceptIndex];
                
                if (!isDeleting) {
                    // НАБОР: Добавляем символ
                    typingTarget.textContent = currentText.substring(0, charIndex + 1);
                    charIndex++;
                } else {
                    // УДАЛЕНИЕ: Убираем символ
                    typingTarget.textContent = currentText.substring(0, charIndex - 1);
                    charIndex--;
                }

                if (charIndex === currentText.length) {
                    // Переключить на удаление
                    isDeleting = true;
                    // Пауза перед удалением
                    setTimeout(typeWriter, 1000); 
                } else if (isDeleting && charIndex === 0) {
                    // Удаление завершено, переходим к следующему слову
                    isDeleting = false;
                    conceptIndex++;
                    
                    if (conceptIndex < concepts.length) {
                        // Пауза перед набором следующего слова
                        setTimeout(typeWriter, 500); 
                    } else {
                        // Все слова набраны, переходим к финальной фазе
                        setTimeout(startFinalPhase, 500);
                        return;
                    }
                } else {
                    // Продолжить набор/удаление
                    const speed = isDeleting ? 50 : 100; // Быстрое удаление, медленный набор
                    setTimeout(typeWriter, speed);
                }
            }

            // Функция Финальной 3D-Вспышки
            function startFinalPhase() {
                // Скрываем курсор и контейнер набора
                cursorTarget.style.display = 'none';
                typingTarget.style.display = 'none';
                
                // Показываем финальное слово
                finalWord.style.opacity = 1;
                finalWord.style.fontSize = '5rem';
                
                // Запускаем 3D-анимацию и смену фона
                setTimeout(() => {
                    finalWord.classList.add('explode');
                    
                    // Резкий переход к белому фону и контенту
                    setTimeout(() => {
                        body.classList.add('white-phase');
                        introContainer.style.display = 'none';
                        
                        // Лого и контент появляются одновременно
                        mainContent.classList.add('active');
                        logo.classList.add('active');
                        // НОВАЯ СТРОКА: Активируем PNG-рамку
                        document.getElementById('overlay-frame').classList.add('active');
                        
                    }, 800); // Тайминг синхронизирован с CSS-анимацией finalExplosion

                }, 200);
            }

            // Инициализация
            typingTarget.style.opacity = 1;
            typeWriter();

        });
    </script>
</body>
</html>
