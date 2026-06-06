<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Config Constructor - Добавь правила в свой конфиг</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            min-height: 100vh;
            padding: 40px 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        
        .card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 24px;
            padding: 30px;
            margin-bottom: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        h1 {
            color: white;
            text-align: center;
            margin-bottom: 10px;
            font-size: 2.5em;
        }
        
        .subtitle {
            text-align: center;
            color: #aaa;
            margin-bottom: 30px;
        }
        
        h2 {
            color: #4CAF50;
            margin-bottom: 20px;
            font-size: 1.5em;
            border-bottom: 2px solid #4CAF50;
            display: inline-block;
        }
        
        h3 {
            color: #ddd;
            margin: 20px 0 15px 0;
        }
        
        .upload-area {
            border: 2px dashed #4CAF50;
            border-radius: 16px;
            padding: 40px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            background: rgba(76, 175, 80, 0.1);
        }
        
        .upload-area:hover {
            background: rgba(76, 175, 80, 0.2);
            border-color: #45a049;
        }
        
        .upload-area.drag-over {
            background: rgba(76, 175, 80, 0.3);
            border-color: #fff;
        }
        
        .file-input {
            display: none;
        }
        
        .upload-icon {
            font-size: 48px;
            margin-bottom: 10px;
        }
        
        .file-status {
            margin-top: 15px;
            padding: 10px;
            border-radius: 8px;
            display: none;
        }
        
        .file-status.success {
            background: rgba(76, 175, 80, 0.3);
            color: #4CAF50;
            display: block;
        }
        
        .file-status.error {
            background: rgba(244, 67, 54, 0.3);
            color: #f44336;
            display: block;
        }
        
        .option-group {
            background: rgba(0, 0, 0, 0.3);
            border-radius: 16px;
            padding: 20px;
            margin-bottom: 25px;
        }
        
        .rules-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 12px;
        }
        
        label {
            display: flex;
            align-items: center;
            margin: 12px 0;
            cursor: pointer;
            color: #eee;
            font-size: 16px;
        }
        
        input[type="checkbox"] {
            margin-right: 12px;
            width: 18px;
            height: 18px;
            cursor: pointer;
        }
        
        button {
            background: linear-gradient(135deg, #4CAF50, #45a049);
            color: white;
            border: none;
            padding: 16px 32px;
            font-size: 18px;
            font-weight: bold;
            border-radius: 50px;
            cursor: pointer;
            width: 100%;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        
        button:hover:not(:disabled) {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }
        
        button:active {
            transform: translateY(0);
        }
        
        button:disabled {
            opacity: 0.5;
            cursor: not-allowed;
        }
        
        .download-area {
            margin-top: 20px;
            text-align: center;
        }
        
        .download-link {
            display: inline-block;
            margin-top: 15px;
            padding: 12px 24px;
            background: #2196F3;
            color: white;
            text-decoration: none;
            border-radius: 50px;
            transition: background 0.3s;
        }
        
        .download-link:hover {
            background: #1976D2;
        }
        
        .status {
            margin-top: 20px;
            padding: 15px;
            border-radius: 12px;
            text-align: center;
            display: none;
        }
        
        .status.loading {
            background: rgba(33, 150, 243, 0.3);
            color: #2196F3;
            display: block;
        }
        
        .status.success {
            background: rgba(76, 175, 80, 0.3);
            color: #4CAF50;
            display: block;
        }
        
        .status.error {
            background: rgba(244, 67, 54, 0.3);
            color: #f44336;
            display: block;
        }
        
        .badge {
            background: #4CAF50;
            color: white;
            padding: 4px 8px;
            border-radius: 8px;
            font-size: 12px;
            margin-left: 10px;
        }
        
        .info-text {
            background: rgba(33, 150, 243, 0.2);
            padding: 10px;
            border-radius: 8px;
            margin-top: 15px;
            font-size: 14px;
            color: #aaa;
        }
        
        footer {
            text-align: center;
            color: #666;
            margin-top: 30px;
        }
        
        @media (max-width: 600px) {
            .card {
                padding: 20px;
            }
            h1 {
                font-size: 1.8em;
            }
        }
    </style>
    <script src="https://cdn.jsdelivr.net/npm/js-yaml@4.1.0/dist/js-yaml.min.js"></script>
</head>
<body>
    <div class="container">
        <h1>⚙️ CONFIG CONSTRUCTOR</h1>
        <div class="subtitle">Загрузите ваш конфиг → добавьте правила → скачайте готовый</div>
        
        <div class="card">
            <h2>📁 ШАГ 1: Загрузите ваш конфиг</h2>
            <div class="upload-area" id="uploadArea">
                <div class="upload-icon">📂</div>
                <div>Нажмите или перетащите файл сюда</div>
                <div style="font-size: 12px; margin-top: 10px; color: #aaa;">Поддерживаются: .yaml, .yml</div>
                <input type="file" id="fileInput" class="file-input" accept=".yaml,.yml">
            </div>
            <div id="fileStatus" class="file-status"></div>
            <div class="info-text">
                💡 Ваш конфиг будет очищен от лишнего, но все ваши прокси и сервера сохранятся
            </div>
        </div>
        
        <div class="card" id="rulesCard" style="display: none;">
            <h2>📦 ШАГ 2: Выберите нужные правила</h2>
            <div class="option-group">
                <div class="rules-grid" id="rulesList">
                    <!-- Правила будут добавлены через JS -->
                </div>
            </div>
            
            <h2>⚙️ ШАГ 3: Настройки обработки</h2>
            <div class="option-group">
                <label>
                    <input type="checkbox" id="keepProxies" checked>
                    ✅ Сохранить мои прокси (из моего конфига)
                </label>
                <label>
                    <input type="checkbox" id="clearProxies">
                    🗑️ Очистить все прокси (оставить только правила)
                </label>
                <label>
                    <input type="checkbox" id="addRuleGroup">
                    📁 Добавить прокси-группу "CustomRules" для новых правил
                </label>
                <label>
                    <input type="checkbox" id="mergeRules" checked>
                    🔄 Объединить с существующими правилами (не удалять старые)
                </label>
            </div>
            
            <button id="processBtn" onclick="processConfig()">🔄 ОБРАБОТАТЬ КОНФИГ</button>
            
            <div id="processStatus" class="status"></div>
            <div class="download-area" id="downloadArea" style="display: none;">
                <a id="downloadLink" class="download-link">📥 Скачать config.yaml с правилами</a>
            </div>
        </div>
        
        <footer>
            🔒 Конфиг обрабатывается локально в вашем браузере<br>
            Никакие данные не отправляются на сервер
        </footer>
    </div>

    <script>
        // Доступные правила
        const availableRules = [
            { id: "youtube", name: "🎬 YouTube", desc: "Обход блокировки YouTube" },
            { id: "netflix", name: "🎥 Netflix", desc: "Доступ к Netflix" },
            { id: "tiktok", name: "📱 TikTok", desc: "Доступ к TikTok" },
            { id: "discord", name: "💬 Discord", desc: "Доступ к Discord" },
            { id: "steam", name: "🎮 Steam", desc: "Игровой трафик Steam" },
            { id: "twitch", name: "📺 Twitch", desc: "Стриминговый сервис" },
            { id: "spotify", name: "🎵 Spotify", desc: "Музыкальный сервис" },
            { id: "telegram", name: "✈️ Telegram", desc: "Мессенджер" }
        ];
        
        let uploadedConfig = null;
        let uploadedConfigText = null;
        
        // Рендерим список правил
        function renderRulesList() {
            const container = document.getElementById('rulesList');
            container.innerHTML = availableRules.map(rule => `
                <label>
                    <input type="checkbox" class="rule-checkbox" value="${rule.id}" checked>
                    <strong>${rule.name}</strong>
                    <span style="font-size: 12px; color: #aaa; margin-left: 8px;">${rule.desc}</span>
                </label>
            `).join('');
        }
        
        // Загрузка файла
        function setupFileUpload() {
            const uploadArea = document.getElementById('uploadArea');
            const fileInput = document.getElementById('fileInput');
            const fileStatus = document.getElementById('fileStatus');
            
            uploadArea.onclick = () => fileInput.click();
            
            uploadArea.ondragover = (e) => {
                e.preventDefault();
                uploadArea.classList.add('drag-over');
            };
            
            uploadArea.ondragleave = () => {
                uploadArea.classList.remove('drag-over');
            };
            
            uploadArea.ondrop = (e) => {
                e.preventDefault();
                uploadArea.classList.remove('drag-over');
                const file = e.dataTransfer.files[0];
                if (file) handleFile(file);
            };
            
            fileInput.onchange = (e) => {
                const file = e.target.files[0];
                if (file) handleFile(file);
            };
        }
        
        async function handleFile(file) {
            const fileStatus = document.getElementById('fileStatus');
            
            if (!file.name.match(/\.(yaml|yml)$/)) {
                fileStatus.className = 'file-status error';
                fileStatus.textContent = '❌ Пожалуйста, загрузите YAML файл';
                return;
            }
            
            try {
                const text = await file.text();
                const config = jsyaml.load(text);
                
                // Проверяем что это валидный конфиг
                if (!config || typeof config !== 'object') {
                    throw new Error('Невалидный YAML файл');
                }
                
                uploadedConfig = config;
                uploadedConfigText = text;
                
                fileStatus.className = 'file-status success';
                fileStatus.textContent = `✅ Загружено: ${file.name} (${Object.keys(config).length} секций)`;
                
                // Показываем карточку с правилами
                document.getElementById('rulesCard').style.display = 'block';
                renderRulesList();
                
            } catch(error) {
                fileStatus.className = 'file-status error';
                fileStatus.textContent = `❌ Ошибка: ${error.message}`;
            }
        }
        
        // Очистка конфига от лишнего
        function cleanConfig(config) {
            const cleaned = {};
            
            // Сохраняем только нужные секции
            const allowedSections = ['proxies', 'proxy-groups', 'rules', 'rule-providers', 'warp-common'];
            
            for (const section of allowedSections) {
                if (config[section]) {
                    cleaned[section] = config[section];
                }
            }
            
            // Если есть warp-common, сохраняем и его
            if (config['warp-common']) {
                cleaned['warp-common'] = config['warp-common'];
            }
            
            return cleaned;
        }
        
        // Получение выбранных правил
        async function getSelectedRules() {
            const selected = [];
            const checkboxes = document.querySelectorAll('.rule-checkbox:checked');
            
            for (const cb of checkboxes) {
                try {
                    const response = await fetch(`rules/${cb.value}.yaml`);
                    if (response.ok) {
                        const ruleContent = await response.text();
                        const ruleObj = jsyaml.load(ruleContent);
                        selected.push(ruleObj);
                    } else {
                        console.log(`Правила для ${cb.value} не найдены`);
                    }
                } catch(e) {
                    console.error(`Ошибка загрузки ${cb.value}:`, e);
                }
            }
            
            return selected;
        }
        
        // Объединение правил
        function mergeRules(existingRules, newRules, mergeMode) {
            if (mergeMode) {
                // Объединяем с существующими
                return [...(existingRules || []), ...newRules];
            } else {
                // Заменяем существующие
                return newRules;
            }
        }
        
        // Основная функция обработки
        async function processConfig() {
            if (!uploadedConfig) {
                alert('Сначала загрузите конфиг');
                return;
            }
            
            const processStatus = document.getElementById('processStatus');
            const processBtn = document.getElementById('processBtn');
            const downloadArea = document.getElementById('downloadArea');
            
            processStatus.className = 'status loading';
            processStatus.textContent = '⏳ Обработка конфига...';
            processBtn.disabled = true;
            
            try {
                // Получаем настройки
                const keepProxies = document.getElementById('keepProxies').checked;
                const clearProxies = document.getElementById('clearProxies').checked;
                const addRuleGroup = document.getElementById('addRuleGroup').checked;
                const mergeRulesMode = document.getElementById('mergeRules').checked;
                
                // 1. Очищаем конфиг
                let finalConfig = cleanConfig(uploadedConfig);
                
                // 2. Обрабатываем прокси
                if (clearProxies) {
                    delete finalConfig.proxies;
                    delete finalConfig['proxy-groups'];
                } else if (!keepProxies) {
                    // По умолчанию сохраняем прокси
                    // Ничего не делаем
                }
                
                // 3. Получаем выбранные правила
                const selectedRules = await getSelectedRules();
                
                // 4. Объединяем правила
                let newRulesList = [];
                let newRuleProviders = {};
                
                for (const ruleObj of selectedRules) {
                    if (ruleObj.rules) {
                        newRulesList.push(...ruleObj.rules);
                    }
                    if (ruleObj['rule-providers']) {
                        newRuleProviders = {...newRuleProviders, ...ruleObj['rule-providers']};
                    }
                }
                
                // 5. Добавляем правила в конфиг
                finalConfig.rules = mergeRules(finalConfig.rules, newRulesList, mergeRulesMode);
                
                // 6. Добавляем rule-providers
                if (Object.keys(newRuleProviders).length > 0) {
                    finalConfig['rule-providers'] = {
                        ...(finalConfig['rule-providers'] || {}),
                        ...newRuleProviders
                    };
                }
                
                // 7. Добавляем прокси-группу для правил если нужно
                if (addRuleGroup && newRulesList.length > 0) {
                    const ruleGroup = {
                        name: "CustomRules",
                        type: "select",
                        proxies: ["DIRECT", "PROXY", "Cloudflare"]
                    };
                    
                    if (!finalConfig['proxy-groups']) {
                        finalConfig['proxy-groups'] = [];
                    }
                    finalConfig['proxy-groups'].push(ruleGroup);
                }
                
                // 8. Конвертируем в YAML
                const finalYaml = jsyaml.dump(finalConfig, {
                    indent: 2,
                    lineWidth: -1,
                    noRefs: true,
                    sortKeys: false
                });
                
                // 9. Предлагаем скачать
                const blob = new Blob([finalYaml], {type: 'text/yaml'});
                const url = URL.createObjectURL(blob);
                const downloadLink = document.getElementById('downloadLink');
                
                downloadLink.href = url;
                downloadLink.download = 'config_with_rules.yaml';
                
                downloadArea.style.display = 'block';
                
                processStatus.className = 'status success';
                processStatus.textContent = `✅ Конфиг обработан! Добавлено правил: ${newRulesList.length}`;
                
            } catch(error) {
                console.error(error);
                processStatus.className = 'status error';
                processStatus.textContent = `❌ Ошибка: ${error.message}`;
            } finally {
                processBtn.disabled = false;
            }
        }
        
        // Инициализация
        setupFileUpload();
    </script>
</body>
</html>
