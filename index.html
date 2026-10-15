<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JEMPO AI - Recomendador Simple</title>
    <style>
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --bg: #f8fafc;
            --card-bg: #ffffff;
            --text: #1e293b;
            --text-light: #64748b;
            --success: #10b981;
            --warning: #f59e0b;
            --danger: #ef4444;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 30px;
        }

        header h1 {
            color: var(--primary);
            font-size: 2rem;
            margin-bottom: 10px;
        }

        header p {
            color: var(--text-light);
        }

        .card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 24px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 16px;
        }

        label {
            display: block;
            font-weight: 600;
            margin-bottom: 6px;
            color: var(--text);
        }

        input, select {
            width: 100%;
            padding: 10px 12px;
            border: 1px solid #cbd5e1;
            border-radius: 8px;
            font-size: 1rem;
            transition: border-color 0.2s;
        }

        input:focus, select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
        }

        button {
            width: 100%;
            padding: 12px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.2s;
        }

        button:hover {
            background-color: var(--primary-dark);
        }

        .result-section {
            display: none;
            animation: fadeIn 0.4s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .budget-status {
            padding: 12px;
            border-radius: 8px;
            font-weight: 600;
            text-align: center;
            margin-bottom: 20px;
        }

        .budget-ok { background-color: #d1fae5; color: #065f46; }
        .budget-warn { background-color: #fef3c7; color: #92400e; }
        .budget-fail { background-color: #fee2e2; color: #991b1b; }

        .spec-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 16px;
            margin-bottom: 20px;
        }

        .spec-item {
            background: #f1f5f9;
            padding: 12px;
            border-radius: 8px;
        }

        .spec-item strong {
            display: block;
            color: var(--primary);
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            margin-bottom: 4px;
        }

        .software-list, .security-tip {
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid #e2e8f0;
        }

        .software-list h3, .security-tip h3 {
            font-size: 1.1rem;
            margin-bottom: 10px;
        }

        .software-list ul {
            list-style-position: inside;
            color: var(--text-light);
        }

        .software-list li {
            margin-bottom: 6px;
        }

        .security-tip {
            background-color: #eff6ff;
            border-left: 4px solid var(--primary);
            padding: 16px;
            border-radius: 0 8px 8px 0;
        }

        .laptop-note {
            background-color: #fff7ed;
            border-left: 4px solid var(--warning);
            padding: 12px;
            border-radius: 0 8px 8px 0;
            margin-bottom: 16px;
            font-size: 0.9rem;
            color: #9a3412;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>⚡ JEMPO AI Simple</h1>
        <p>Recomendador inteligente de hardware y software. Sin complicaciones.</p>
    </header>

    <div class="card">
        <div class="form-group">
            <label for="presupuesto">Presupuesto aproximado (S/)</label>
            <input type="number" id="presupuesto" placeholder="Ej: 2500" min="0">
        </div>

        <div class="form-group">
            <label for="uso">Uso principal</label>
            <select id="uso">
                <option value="Estudio y oficina">Estudio y oficina</option>
                <option value="Gaming">Gaming</option>
                <option value="Diseño y edición">Diseño y edición</option>
                <option value="Programación">Programación</option>
                <option value="Ciberseguridad">Ciberseguridad</option>
            </select>
        </div>

        <div class="form-group">
            <label for="nivel">Nivel de exigencia</label>
            <select id="nivel">
                <option value="Básico">Básico</option>
                <option value="Intermedio">Intermedio</option>
                <option value="Alto">Alto</option>
            </select>
        </div>

        <div class="form-group">
            <label for="tipo">Tipo de equipo</label>
            <select id="tipo">
                <option value="PC de escritorio">PC de escritorio</option>
                <option value="Laptop">Laptop</option>
            </select>
        </div>

        <button onclick="generarRecomendacion()">Generar Recomendación</button>
    </div>

    <div id="resultado" class="card result-section">
        <div id="laptopNote" class="laptop-note" style="display: none;">
            💡 <strong>Nota para Laptops:</strong> Las especificaciones son de referencia. En laptops, el CPU y GPU suelen venir soldados y no son actualizables. Busca modelos comerciales que se acerquen a estas características.
        </div>

        <div id="budgetStatus" class="budget-status"></div>

        <h2 style="margin-bottom: 16px; font-size: 1.25rem;">Configuración Recomendada</h2>
        <div class="spec-grid" id="specGrid">
            <!-- Las especificaciones se insertan aquí con JS -->
        </div>

        <div class="software-list">
            <h3>💿 Software Sugerido</h3>
            <ul id="softwareList"></ul>
        </div>

        <div class="security-tip">
            <h3>🛡️ Consejo de Seguridad Digital</h3>
            <p id="securityTip"></p>
        </div>
        
        <button onclick="window.print()" style="margin-top: 20px; background-color: #64748b;">🖨️ Imprimir / Guardar como PDF</button>
    </div>
</div>

<script>
    // Base de datos simplificada de recomendaciones
    const baseDeDatos = {
        "Estudio y oficina": {
            "Básico": {
                cpu: "Intel Core i3-12100 o AMD Ryzen 3 4100",
                gpu: "Gráficos integrados (Intel UHD / Radeon Vega)",
                ram: "8 GB DDR4",
                almacenamiento: "SSD NVMe 256 GB",
                mainboard: "Placa base A320 / H510",
                psu: "Fuente 450W-500W 80 Plus",
                case: "Gabinete Micro ATX básico",
                software: ["Windows 11 / Linux Mint", "LibreOffice o Google Workspace", "Navegador web (Chrome/Firefox)"],
                precioEstimado: 1200
            },
            "Intermedio": {
                cpu: "Intel Core i5-12400 o AMD Ryzen 5 5600G",
                gpu: "Gráficos integrados Radeon Vega o GTX 1650",
                ram: "16 GB DDR4 3200 MHz",
                almacenamiento: "SSD NVMe M.2 500 GB",
                mainboard: "Placa base B450 / B660",
                psu: "Fuente 550W 80 Plus Bronze",
                case: "Gabinete ATX/Micro ATX con buen flujo de aire",
                software: ["Windows 11", "Microsoft 365", "Zoom / Teams", "Notion"],
                precioEstimado: 1800
            },
            "Alto": {
                cpu: "Intel Core i7-12700 o AMD Ryzen 7 5700X",
                gpu: "RTX 4060 8 GB (para multitarea pesada)",
                ram: "32 GB DDR4/DDR5",
                almacenamiento: "SSD NVMe M.2 1 TB",
                mainboard: "Placa base B660 / B550 con WiFi",
                psu: "Fuente 650W 80 Plus Gold",
                case: "Gabinete ATX premium con alto flujo",
                software: ["Windows 11 Pro", "Suite de Office avanzada", "Power BI Desktop", "Gestor de contraseñas (Bitwarden)"],
                precioEstimado: 3000
            }
        },
        "Gaming": {
            "Básico": {
                cpu: "AMD Ryzen 5 5600G o Intel Core i3-12100F",
                gpu: "GTX 1650 4 GB o Radeon RX 580 8 GB",
                ram: "16 GB DDR4 3200 MHz",
                almacenamiento: "SSD NVMe M.2 500 GB",
                mainboard: "Placa base B450 / H610",
                psu: "Fuente 550W 80 Plus Bronze",
                case: "Gabinete Micro ATX con ventilación",
                software: ["Windows 11", "Steam / Epic Games", "Discord", "Drivers oficiales de GPU"],
                precioEstimado: 2000
            },
            "Intermedio": {
                cpu: "AMD Ryzen 5 5600 o Intel Core i5-12400F",
                gpu: "Radeon RX 6600 XT 8 GB o RTX 4060 8 GB",
                ram: "16 GB o 32 GB DDR4 3200 MHz",
                almacenamiento: "SSD NVMe M.2 1 TB",
                mainboard: "Placa base B550 / B660",
                psu: "Fuente 650W 80 Plus Bronze/Gold",
                case: "Gabinete ATX Airflow",
                software: ["Windows 11", "Steam", "Discord", "MSI Afterburner", "OBS Studio"],
                precioEstimado: 3500
            },
            "Alto": {
                cpu: "AMD Ryzen 7 5700X o Intel Core i7-12700F",
                gpu: "RTX 4060 Ti o RTX 4070",
                ram: "32 GB DDR5 5600 MHz",
                almacenamiento: "SSD NVMe M.2 2 TB",
                mainboard: "Placa base B650 / B760",
                psu: "Fuente 750W - 850W 80 Plus Gold",
                case: "Gabinete ATX premium con alto flujo",
                software: ["Windows 11", "Steam", "Discord", "HWiNFO", "CapFrameX"],
                precioEstimado: 5500
            }
        },
        "Diseño y edición": {
            "Básico": {
                cpu: "AMD Ryzen 5 5600G o Intel Core i5-12400",
                gpu: "Gráficos integrados o GTX 1650",
                ram: "16 GB DDR4",
                almacenamiento: "SSD NVMe M.2 500 GB",
                mainboard: "Placa base B450 / B660",
                psu: "Fuente 550W 80 Plus",
                case: "Gabinete Micro ATX",
                software: ["Windows 11", "Canva", "GIMP / Photopea", "Inkscape"],
                precioEstimado: 2200
            },
            "Intermedio": {
                cpu: "AMD Ryzen 5 5600 o Intel Core i5-12400F",
                gpu: "RTX 4060 8 GB o RX 6600 XT",
                ram: "32 GB DDR4 3200 MHz",
                almacenamiento: "SSD NVMe M.2 1 TB",
                mainboard: "Placa base B550 / B660",
                psu: "Fuente 650W 80 Plus Gold",
                case: "Gabinete ATX Airflow",
                software: ["Windows 11", "Adobe Photoshop / Illustrator", "DaVinci Resolve", "Figma"],
                precioEstimado: 4000
            },
            "Alto": {
                cpu: "AMD Ryzen 7 5700X o Intel Core i7-12700F",
                gpu: "RTX 4070 o superior",
                ram: "64 GB DDR5",
                almacenamiento: "SSD NVMe M.2 2 TB",
                mainboard: "Placa base B650 / B760",
                psu: "Fuente 750W - 850W 80 Plus Gold",
                case: "Gabinete ATX premium",
                software: ["Windows 11 Pro", "Adobe Creative Cloud", "Blender", "DaVinci Resolve Studio"],
                precioEstimado: 6500
            }
        },
        "Programación": {
            "Básico": {
                cpu: "AMD Ryzen 5 5600G o Intel Core i3-12100",
                gpu: "Gráficos integrados",
                ram: "16 GB DDR4",
                almacenamiento: "SSD NVMe M.2 500 GB",
                mainboard: "Placa base A520 / H610",
                psu: "Fuente 500W 80 Plus",
                case: "Gabinete básico",
                software: ["Windows 11 / Linux", "Visual Studio Code", "Git / GitHub", "Navegador web"],
                precioEstimado: 1800
            },
            "Intermedio": {
                cpu: "AMD Ryzen 5 5600 o Intel Core i5-12400",
                gpu: "Gráficos integrados o GPU básica",
                ram: "16 GB o 32 GB DDR4",
                almacenamiento: "SSD NVMe M.2 1 TB",
                mainboard: "Placa base B550 / B660",
                psu: "Fuente 550W-650W 80 Plus",
                case: "Gabinete ATX/Micro ATX",
                software: ["Windows 11 / Linux", "VS Code", "Docker Desktop", "XAMPP", "DBeaver"],
                precioEstimado: 2800
            },
            "Alto": {
                cpu: "AMD Ryzen 7 5700X o Intel Core i7-12700",
                gpu: "RTX 4060 (para IA local o CUDA)",
                ram: "32 GB o 64 GB DDR5",
                almacenamiento: "SSD NVMe M.2 2 TB",
                mainboard: "Placa base B650 / B760",
                psu: "Fuente 750W 80 Plus Gold",
                case: "Gabinete ATX premium",
                software: ["Windows 11 Pro / Linux", "IntelliJ IDEA / PyCharm", "Docker", "WSL2", "Postman"],
                precioEstimado: 5000
            }
        },
        "Ciberseguridad": {
            "Básico": {
                cpu: "AMD Ryzen 5 5600G o Intel Core i5-12400",
                gpu: "Gráficos integrados",
                ram: "16 GB DDR4",
                almacenamiento: "SSD NVMe M.2 500 GB",
                mainboard: "Placa base B450 / B660",
                psu: "Fuente 550W 80 Plus",
                case: "Gabinete Micro ATX",
                software: ["Windows 11 / Linux Mint", "VirtualBox", "Wireshark", "Nmap"],
                precioEstimado: 2000
            },
            "Intermedio": {
                cpu: "AMD Ryzen 5 5600 o Intel Core i5-12400",
                gpu: "Gráficos integrados",
                ram: "32 GB DDR4",
                almacenamiento: "SSD NVMe M.2 1 TB",
                mainboard: "Placa base B550 / B660",
                psu: "Fuente 650W 80 Plus Bronze",
                case: "Gabinete ATX Airflow",
                software: ["Kali Linux (en VM)", "VirtualBox", "Burp Suite Community", "Sysinternals"],
                precioEstimado: 3200
            },
            "Alto": {
                cpu: "AMD Ryzen 7 5700X o Intel Core i7-12700",
                gpu: "GPU dedicada (opcional, para laboratorios de IA)",
                ram: "64 GB DDR5",
                almacenamiento: "SSD NVMe M.2 2 TB",
                mainboard: "Placa base B650 / B760",
                psu: "Fuente 750W - 850W 80 Plus Gold",
                case: "Gabinete ATX premium",
                software: ["Kali Linux", "Wazuh", "GNS3 / EVE-NG", "Metasploit Framework"],
                precioEstimado: 5500
            }
        }
    };

    const tipsSeguridad = [
        "Usa un gestor de contraseñas (como Bitwarden o KeePassXC) y activa la autenticación en dos pasos (2FA) en todas tus cuentas importantes.",
        "Mantén siempre tu sistema operativo, navegadores y drivers actualizados para parchar vulnerabilidades de seguridad.",
        "Realiza copias de seguridad (backups) periódicas de tus archivos importantes en un disco externo o en la nube (Regla 3-2-1).",
        "Nunca descargues software 'crackeado' o activadores, ya que son la principal fuente de malware y robo de información."
    ];

    function generarRecomendacion() {
        const presupuesto = parseFloat(document.getElementById('presupuesto').value) || 0;
        const uso = document.getElementById('uso').value;
        const nivel = document.getElementById('nivel').value;
        const tipo = document.getElementById('tipo').value;

        const recomendacion = baseDeDatos[uso][nivel];
        const precioEstimado = recomendacion.precioEstimado;
        
        // Mostrar sección de resultados
        const resultadoDiv = document.getElementById('resultado');
        resultadoDiv.style.display = 'block';
        
        // Nota para laptops
        document.getElementById('laptopNote').style.display = (tipo === 'Laptop') ? 'block' : 'none';

        // Estado del presupuesto
        const budgetStatus = document.getElementById('budgetStatus');
        if (presupuesto === 0) {
            budgetStatus.className = 'budget-status budget-warn';
            budgetStatus.innerHTML = `⚠️ No ingresaste un presupuesto. El precio estimado de esta configuración es de <strong>S/ ${precioEstimado}</strong>.`;
        } else if (presupuesto >= precioEstimado) {
            const sobrante = presupuesto - precioEstimado;
            budgetStatus.className = 'budget-status budget-ok';
            budgetStatus.innerHTML = `✅ ¡Presupuesto suficiente! Te sobran aproximadamente <strong>S/ ${sobrante}</strong>.`;
        } else {
            const faltante = precioEstimado - presupuesto;
            budgetStatus.className = 'budget-status budget-fail';
            budgetStatus.innerHTML = `❌ Presupuesto ajustado. Te faltan aproximadamente <strong>S/ ${faltante}</strong>. Considera bajar el nivel de exigencia o priorizar componentes.`;
        }

        // Generar grid de especificaciones
        const specGrid = document.getElementById('specGrid');
        specGrid.innerHTML = `
            <div class="spec-item"><strong>Procesador (CPU)</strong>${recomendacion.cpu}</div>
            <div class="spec-item"><strong>Tarjeta Gráfica (GPU)</strong>${recomendacion.gpu}</div>
            <div class="spec-item"><strong>Memoria RAM</strong>${recomendacion.ram}</div>
            <div class="spec-item"><strong>Almacenamiento</strong>${recomendacion.almacenamiento}</div>
            <div class="spec-item"><strong>Placa Madre</strong>${recomendacion.mainboard}</div>
            <div class="spec-item"><strong>Fuente de Poder</strong>${recomendacion.psu}</div>
            <div class="spec-item"><strong>Gabinete</strong>${recomendacion.case}</div>
            <div class="spec-item"><strong>Precio Estimado</strong>S/ ${precioEstimado} (Referencial)</div>
        `;

        // Generar lista de software
        const softwareList = document.getElementById('softwareList');
        softwareList.innerHTML = recomendacion.software.map(sw => `<li>${sw}</li>`).join('');

        // Tip de seguridad aleatorio
        const tipAleatorio = tipsSeguridad[Math.floor(Math.random() * tipsSeguridad.length)];
        document.getElementById('securityTip').textContent = tipAleatorio;

        // Scroll suave hacia el resultado
        resultadoDiv.scrollIntoView({ behavior: 'smooth', block: 'start' });
    }
</script>

</body>
</html>
