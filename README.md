<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Общее собрание — Комсомольская, 138</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Segoe UI', Roboto, Arial, sans-serif;
            background: #f2f5f9;
            color: #1e2a3a;
            padding: 30px 20px;
            display: flex;
            justify-content: center;
        }
        .container {
            max-width: 1100px;
            width: 100%;
            background: #ffffff;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.08);
            padding: 40px 45px;
        }
        h1 {
            font-size: 32px;
            font-weight: 700;
            color: #0b2b4a;
            margin-bottom: 6px;
            letter-spacing: -0.5px;
        }
        .subhead {
            font-size: 18px;
            color: #3d5a78;
            border-bottom: 3px solid #2b6a9e;
            padding-bottom: 15px;
            margin-bottom: 30px;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        .badge {
            background: #2b6a9e;
            color: white;
            padding: 6px 18px;
            border-radius: 30px;
            font-weight: 600;
            font-size: 15px;
        }
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin: 25px 0;
        }
        .info-card {
            background: #f8fafc;
            border-radius: 14px;
            padding: 20px 25px;
            border-left: 6px solid #2b6a9e;
        }
        .info-card h3 {
            font-size: 18px;
            font-weight: 600;
            margin-bottom: 10px;
            color: #0b2b4a;
        }
        .info-card p, .info-card li {
            font-size: 15px;
            line-height: 1.6;
            color: #1e3b5a;
        }
        .info-card ul {
            list-style: none;
            padding-left: 0;
        }
        .info-card ul li {
            padding: 4px 0;
            border-bottom: 1px dashed #dce3ec;
        }
        .info-card ul li:last-child {
            border-bottom: none;
        }
        .highlight {
            background: #e8f0fe;
            border-radius: 12px;
            padding: 18px 22px;
            margin: 20px 0;
        }
        .highlight strong {
            color: #0b2b4a;
        }
        .table-wrap {
            overflow-x: auto;
            margin: 25px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 15px;
        }
        th {
            background: #1e3a5e;
            color: white;
            padding: 12px 15px;
            text-align: left;
            font-weight: 600;
        }
        td {
            padding: 12px 15px;
            border-bottom: 1px solid #dfe6ef;
        }
        tr:last-child td {
            border-bottom: none;
        }
        .number {
            font-weight: 700;
            color: #0b2b4a;
        }
        .green {
            color: #1e7b4c;
        }
        .red {
            color: #b13e3e;
        }
        .calc-box {
            background: #f0f4fa;
            border-radius: 14px;
            padding: 20px 25px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            margin: 20px 0;
        }
        .calc-item {
            flex: 1 1 200px;
            margin: 8px 0;
        }
        .calc-item .label {
            font-size: 14px;
            color: #4d6a8c;
        }
        .calc-item .value {
            font-size: 24px;
            font-weight: 700;
            color: #0b2b4a;
        }
        .btn {
            background: #2b6a9e;
            color: white;
            border: none;
            padding: 12px 28px;
            border-radius: 40px;
            font-weight: 600;
            font-size: 16px;
            cursor: default;
            display: inline-block;
        }
        .btn-outline {
            background: transparent;
            border: 2px solid #2b6a9e;
            color: #2b6a9e;
        }
        .footer {
            margin-top: 35px;
            padding-top: 20px;
            border-top: 2px solid #dfe6ef;
            font-size: 14px;
            color: #4d6a8c;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        .footer a {
            color: #2b6a9e;
            text-decoration: none;
        }
        .bullet-list {
            list-style: none;
            padding-left: 0;
        }
        .bullet-list li::before {
            content: "✓ ";
            color: #2b6a9e;
            font-weight: 700;
        }
        .finance-split {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin: 20px 0;
        }
        .finance-split > div {
            flex: 1;
            min-width: 200px;
            background: #f8fafc;
            border-radius: 14px;
            padding: 18px 22px;
            text-align: center;
        }
        .finance-split .big-number {
            font-size: 32px;
            font-weight: 700;
            color: #0b2b4a;
        }
        .finance-split .desc {
            font-size: 15px;
            color: #3d5a78;
            margin-top: 6px;
        }
        .example-block {
            background: #eef3f9;
            border-radius: 14px;
            padding: 18px 25px;
            margin: 15px 0;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .example-block .item {
            flex: 1;
            min-width: 150px;
            padding: 6px 0;
        }
        .legal-note {
            background: #fff8e7;
            border-left: 6px solid #b68b40;
            border-radius: 14px;
            padding: 20px 25px;
            margin: 25px 0;
            font-size: 15px;
            line-height: 1.7;
            color: #3d3a2e;
        }
        .legal-note strong {
            color: #7a5d1a;
        }
        @media (max-width: 700px) {
            .container {
                padding: 20px;
            }
            .grid-2 {
                grid-template-columns: 1fr;
            }
            .calc-box {
                flex-direction: column;
                align-items: stretch;
            }
            .finance-split {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
<div class="container">

    <!-- ШАПКА -->
    <h1>🏢 Общее собрание собственников</h1>
    <div class="subhead">
        <span><strong>г. Уфа, ул. Комсомольская, д. 138</strong></span>
        <span class="badge">Инициатор: УК «Октябрьский жилищник»</span>
    </div>

    <!-- ДАТЫ И МЕСТО -->
    <div class="grid-2">
        <div class="info-card">
            <h3>📅 Когда и где</h3>
            <p><strong>Очная часть:</strong> 7 июля 2026 г. в 20:00<br>
            <span style="color:#3d5a78;">📍 перед 3-м подъездом</span></p>
            <p><strong>Заочное голосование:</strong> с 08.07.2026 по 26.07.2026 до 19:00<br>
            <strong>Приём бюллетеней:</strong> до 26.07.2026 19:00 в ящике №104 (3-й подъезд)</p>
            <p><strong>Подсчёт голосов:</strong> 26.07.2026 в 19:30</p>
        </div>
        <div class="info-card">
            <h3>📄 Ознакомление с документами</h3>
            <p>📍 Офис УК: ул. Российская, д. 41/3, пн–пт с 08:30 до 17:30</p>
            <p>📞 По запросу: <a href="tel:+79876267822">+7 (987) 626-78-22</a></p>
            <p>📎 В день собрания перед началом</p>
            <p style="margin-top:10px;font-size:14px;color:#4d6a8c;">Объявление размещено 26.06.2026 (за 10 дней до собрания)</p>
        </div>
    </div>

    <!-- ПОВЕСТКА ДНЯ -->
    <div class="highlight">
        <h3 style="margin-bottom:10px;">📋 Повестка дня (13 вопросов)</h3>
        <div style="display:grid; grid-template-columns:1fr 1fr; gap:6px 25px; font-size:15px; line-height:1.7;">
            <div>1. Избрать председателя, секретаря, счётную комиссию</div>
            <div>2. Выбрать способ управления – УО</div>
            <div>3. Выбрать УК – ООО УК «Октябрьский жилищник»</div>
            <div>4. Утвердить проект договора управления</div>
            <div>5. Заключить договор управления</div>
            <div><strong>6. Установить тариф на содержание и ремонт в размере 28,00 руб./кв.м (вместо текущего 22,34 руб./кв.м)</strong></div>
            <div><strong style="color:#0b2b4a;">7. Ремонт первых этажей (подъезды 1–4)</strong></div>
            <div><strong style="color:#0b2b4a;">8. Источник финансирования – статья «содержание»</strong></div>
            <div><strong style="color:#0b2b4a;">9. Утвердить смету 1 346 000 руб., разрешить УК заключить договор подряда</strong></div>
            <div>10. Уполномочить лицо на подписание договора</div>
            <div>11. Оплата КР на ОДН по факту (без корректировки)</div>
            <div>12. Избрать совет дома</div>
            <div style="grid-column: span 2;">13. Определить место хранения протокола и материалов</div>
        </div>
    </div>

    <!-- ГЛАВНОЕ: ФИНАНСОВЫЙ РАСЧЁТ -->
    <h2 style="margin: 30px 0 15px 0; font-size:26px;">💰 Финансовые параметры ремонта</h2>

    <div class="table-wrap">
        <table>
            <tr><th>Показатель</th><th>Значение</th></tr>
            <tr><td>Общая жилая площадь дома</td><td><span class="number">7 840</span> м²</td></tr>
            <tr><td>Стоимость ремонта первых этажей (1–4 подъезды)</td><td><span class="number">1 346 000</span> руб.</td></tr>
            <tr><td>Текущий тариф (старый)</td><td><span class="number">22,34</span> руб./м²</td></tr>
            <tr><td>Предлагаемый тариф (новый)</td><td><span class="number">28,00</span> руб./м²</td></tr>
            <tr><td>Увеличение тарифа</td><td><span class="number green">+5,66</span> руб./м²</td></tr>
            <tr><td>Срок действия нового тарифа</td><td><span class="number">1 год (временно)</span></td></tr>
        </table>
    </div>

    <!-- Расчёт сборов -->
    <div class="calc-box">
        <div class="calc-item">
            <div class="label">Сбор в месяц (по старому тарифу)</div>
            <div class="value">175 145,60 ₽</div>
        </div>
        <div class="calc-item">
            <div class="label">Сбор в месяц (по новому тарифу)</div>
            <div class="value" style="color:#1e7b4c;">219 520,00 ₽</div>
        </div>
        <div class="calc-item">
            <div class="label">Увеличение сбора в месяц</div>
            <div class="value" style="color:#b13e3e;">+44 374,40 ₽</div>
        </div>
        <div class="calc-item">
            <div class="label">Увеличение сбора за 1 год</div>
            <div class="value" style="color:#b13e3e;">+532 492,80 ₽</div>
        </div>
    </div>

    <!-- Как финансируется ремонт? -->
    <div style="background:#eaf0fa; border-radius:14px; padding:20px 25px; margin:20px 0;">
        <h3 style="margin-bottom:12px;">🧾 Как финансируется ремонт?</h3>
        <div class="finance-split">
            <div style="background:#ffffff; border:2px solid #2b6a9e;">
                <div class="big-number">532 493 ₽</div>
                <div class="desc"><strong>Доп. сбор за 1 год</strong> (повышение тарифа)</div>
                <div style="font-size:14px; color:#4d6a8c;">≈ 39,6% от стоимости ремонта</div>
            </div>
            <div style="background:#ffffff; border:2px solid #1e7b4c;">
                <div class="big-number">813 507 ₽</div>
                <div class="desc"><strong>Из действующего тарифа</strong> (статья «содержание»)</div>
                <div style="font-size:14px; color:#4d6a8c;">≈ 60,4% от стоимости ремонта</div>
            </div>
            <div style="background:#ffffff; border:2px solid #b13e3e;">
                <div class="big-number">1 346 000 ₽</div>
                <div class="desc"><strong>Общая стоимость ремонта</strong></div>
            </div>
        </div>
        <p style="font-size:15px; margin-top:8px; color:#1e3b5a;">
            <strong>Важно:</strong> повышение тарифа вводится <strong>всего на 1 год</strong> для целевого сбора недостающей суммы. 
            После завершения ремонта тариф будет пересмотрен (вернётся к прежнему уровню или будет снижен). 
            Ремонт выполняется <strong>сразу</strong>, а средства собираются постепенно в течение года.
        </p>
    </div>

    <!-- ЮРИДИЧЕСКОЕ ОБОСНОВАНИЕ (НОВЫЙ БЛОК) -->
    <div class="legal-note">
        <h3 style="margin:0 0 8px 0; color:#7a5d1a;">⚖️ Юридическое обоснование необходимости голосования</h3>
        <p>
            <strong>Были направлены официальные обращения</strong> по данному вопросу в Администрацию Президента РФ, 
            Администрацию Главы Республики Башкортостан, Прокуратуру РФ, Прокуратуру РБ, Партию «Единая Россия», 
            Жилкомнадзор, МВД по Октябрьскому району и другие инстанции.
        </p>
        <p style="margin-top:10px;">
            <strong>В ответ на все обращения поступило единое законодательно обоснованное решение:</strong>
        </p>
        <ul style="margin:8px 0 0 20px; list-style:disc; line-height:1.8;">
            <li><strong>Ремонт общего имущества проводится <span style="color:#b13e3e;">только по решению собственников</span></strong> – ранее голосование не проводилось, поэтому ремонт не мог быть начат.</li>
            <li><strong>Источник финансирования – тариф «содержание и ремонт».</strong> Однако действующий тариф является <strong>муниципальным (минимальным)</strong>, он предусматривает лишь <strong>локальный, точечный ремонт</strong> (замена одной плитки, покраска одной стены), а не комплексное обновление подъездов.</li>
            <li>Для полноценного ремонта необходимо <strong>волеизъявление собственников</strong> и установление экономически обоснованного тарифа (пусть и временно).</li>
        </ul>
        <p style="margin-top:12px; font-style:italic; color:#5a4d2e;">
            Таким образом, единственный законный путь сделать капитальный ремонт первых этажей – <strong>проголосовать «ЗА»</strong> предложенные вопросы повестки.
        </p>
    </div>

    <!-- Примеры для квартир -->
    <div style="display:flex; flex-wrap:wrap; gap:20px; margin:25px 0;">
        <div class="example-block" style="flex:1;">
            <div class="item"><strong>Для квартиры 50 м²:</strong></div>
            <div class="item">Доплата в месяц: 50 × 5,66 = <span class="number">283 ₽</span></div>
            <div class="item">Доплата за год: 283 × 12 = <span class="number">3 396 ₽</span></div>
        </div>
        <div class="example-block" style="flex:1; background:#e4edf7;">
            <div class="item"><strong>Для квартиры 60 м²:</strong></div>
            <div class="item">Доплата в месяц: 60 × 5,66 = <span class="number">339,60 ₽</span></div>
            <div class="item">Доплата за год: 339,60 × 12 = <span class="number">4 075,20 ₽</span></div>
        </div>
    </div>

    <!-- Аргументы для выступления -->
    <div style="background:#f0f7ea; border-radius:14px; padding:20px 25px; margin:25px 0; border-left:6px solid #1e7b4c;">
        <h3 style="margin-bottom:8px;">🗣️ Почему стоит голосовать «ЗА»?</h3>
        <ul style="list-style:none; padding-left:0; font-size:15px; line-height:1.8;">
            <li><strong>✔ Временное повышение</strong> – только на 1 год, затем тариф снижается.</li>
            <li><strong>✔ Прозрачность</strong> – смета утверждена, работы под контролем жильцов.</li>
            <li><strong>✔ Выгода</strong> – ремонт подъездов повышает стоимость квартир на 5–10%.</li>
            <li><strong>✔ Комфорт и безопасность</strong> – устраняются сырость, грибок, улучшается освещение.</li>
            <li><strong>✔ Законность</strong> – ремонт общего имущества – обязанность собственников (ст. 39, 158 ЖК РФ).</li>
        </ul>
        <p style="margin-top:12px; font-weight:600; font-size:17px;">Проголосуйте за ремонт и временное повышение тарифа – сделаем дом лучше!</p>
    </div>

    <!-- КОНТАКТЫ И ПОДПИСЬ -->
    <div class="footer">
        <span>Дата размещения: 26 июня 2026 г.</span>
        <span>Инициатор: ООО УК «Октябрьский жилищник»</span>
        <span>Контакты: <a href="tel:+79876267822">+7 (987) 626-78-22</a></span>
    </div>

    <div style="text-align:right; font-size:13px; color:#8a9cb0; margin-top:20px; border-top:1px solid #dfe6ef; padding-top:15px;">
        Презентация по ссылке – актуально на 28.06.2026
    </div>

</div>
</body>
</html>
