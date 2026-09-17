<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Fuentes Kawaii y Modernas -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@400;500;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
    <!-- MathJax para fórmulas LaTeX -->
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    
    <style>
        :root {
            --bg-page: #faf7f8;
            --card-bg: #ffffff;
            --text-dark: #4a4e69;
            --text-muted: #7a7f9d;
            
            /* Paleta Pastel Kawaii */
            --pink-soft: #ffb7b2;
            --pink-bg: #fff0f3;
            --mint-soft: #b5ead7;
            --mint-bg: #e8f8f5;
            --lavender-soft: #c7ceea;
            --lavender-bg: #f3f0ff;
            --peach-soft: #ffdac1;
            --peach-bg: #fff5eb;
            --yellow-soft: #e2f0cb;
            
            --border-radius: 20px;
            --shadow-kawaii: 0 10px 25px -5px rgba(202, 179, 205, 0.25);
            --shadow-hover: 0 15px 30px -5px rgba(180, 150, 190, 0.35);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            font-family: 'M PLUS Rounded 1c', -apple-system, sans-serif;
            background-color: var(--bg-page);
            color: var(--text-dark);
            line-height: 1.7;
            padding: 40px 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        /* Banner Principal Header */
        header.kawaii-header {
            background: linear-gradient(135deg, var(--pink-soft), var(--lavender-soft));
            border-radius: var(--border-radius);
            padding: 40px 30px;
            text-align: center;
            color: white;
            box-shadow: var(--shadow-kawaii);
            margin-bottom: 35px;
            position: relative;
        }

        header.kawaii-header h1 {
            font-size: 2.2rem;
            font-weight: 800;
            text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 8px;
        }

        header.kawaii-header p {
            font-size: 1.1rem;
            font-weight: 500;
            opacity: 0.95;
        }

        /* Metodología de Estudio en 8 pasos */
        .methodology-card {
            background: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 30px;
            box-shadow: var(--shadow-kawaii);
            border: 2px solid #f0e6ed;
            margin-bottom: 40px;
        }

        .methodology-card h2 {
            font-size: 1.3rem;
            color: #9a8c98;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .method-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 12px 20px;
        }

        .method-item {
            font-size: 0.92rem;
            color: var(--text-dark);
            background: #faf4f8;
            padding: 8px 14px;
            border-radius: 12px;
            border-left: 4px solid var(--pink-soft);
        }

        /* Secciones por Materia */
        .subject-header {
            font-size: 1.7rem;
            font-weight: 800;
            margin: 45px 0 20px 0;
            padding-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 12px;
            border-bottom: 3px dashed #e0d6dd;
        }

        /* Módulos / Cards */
        .kawaii-card {
            background: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--shadow-kawaii);
            border: 1px solid #f5edf2;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .kawaii-card:hover {
            transform: translateY(-3px);
            box-shadow: var(--shadow-hover);
        }

        .badge {
            display: inline-flex;
            align-items: center;
            padding: 5px 14px;
            border-radius: 50px;
            font-size: 0.8rem;
            font-weight: 700;
            letter-spacing: 0.02em;
            margin-bottom: 15px;
        }

        .badge-reconocer { background: var(--mint-bg); color: #2e7d6e; border: 1px solid var(--mint-soft); }
        .badge-entender { background: var(--peach-bg); color: #c86d3b; border: 1px solid var(--peach-soft); }
        .badge-resolver { background: var(--pink-bg); color: #d64550; border: 1px solid var(--pink-soft); }

        .kawaii-card h3 {
            font-size: 1.35rem;
            font-weight: 700;
            color: var(--text-dark);
            margin-bottom: 18px;
        }

        .step-block {
            margin-bottom: 16px;
            font-size: 0.98rem;
        }

        .step-label {
            font-weight: 700;
            color: #6c5ce7;
            display: block;
            margin-bottom: 4px;
        }

        /* Cajas destacadas pastel */
        .example-box {
            background: var(--lavender-bg);
            border-left: 5px solid var(--lavender-soft);
            padding: 18px 22px;
            border-radius: 14px;
            margin: 18px 0;
            font-size: 0.95rem;
        }

        .warning-box {
            background: #fff8f0;
            border-left: 5px solid var(--peach-soft);
            padding: 16px 20px;
            border-radius: 14px;
            margin: 18px 0;
            font-size: 0.93rem;
            color: #a0522d;
        }

        .synoptic-box {
            background: #fafafa;
            border: 2px dashed var(--lavender-soft);
            padding: 20px;
            border-radius: 16px;
            margin-top: 22px;
            font-size: 0.93rem;
        }

        .synoptic-box strong {
            color: #6c5ce7;
            display: block;
            margin-bottom: 10px;
        }

        .synoptic-box ul {
            list-style: none;
            padding-left: 0;
        }

        .synoptic-box li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 8px;
        }

        .synoptic-box li::before {
            content: "✦";
            color: var(--pink-soft);
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* Bloques de Código */
        .code-container {
            background: #282a36;
            color: #f8f8f2;
            padding: 18px 22px;
            border-radius: 14px;
            font-family: 'JetBrains Mono', monospace;
            font-size: 0.88rem;
            overflow-x: auto;
            margin: 14px 0;
            box-shadow: inset 0 2px 6px rgba(0,0,0,0.2);
        }

        /* Tabla Estilizada */
        table {
            width: 100%;
            border-collapse: separate;
            border-spacing: 0;
            margin: 25px 0;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow-kawaii);
            border: 1px solid #f0e6ed;
        }

        th, td {
            padding: 14px 18px;
            text-align: left;
            font-size: 0.92rem;
        }

        th {
            background: var(--lavender-bg);
            color: #5a4b81;
            font-weight: 700;
        }

        td {
            background: var(--card-bg);
            border-bottom: 1px solid #f5edf2;
        }

        tr:last-child td {
            border-bottom: none;
        }

        /* Autoevaluación */
        .self-eval {
            background: #f8f9fa;
            border-radius: 12px;
            padding: 12px 18px;
            margin-top: 15px;
            font-size: 0.88rem;
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        @media print {
            body { background: white; padding: 0; }
            .kawaii-card, .methodology-card { box-shadow: none; border: 1px solid #ddd; page-break-inside: avoid; }
            .subject-header { page-break-before: always; }
        }
    </style>
</head>
<body>

<div class="container">

    <header class="kawaii-header">
        <h1>(⁠◕⁠‿⁠◕⁠✿⁠) Cuadernillo de Estudio Integral</h1>
        <p>Ciencias Exactas, Biología & Programación • Guía Práctica Autónomica</p>
    </header>

    <!-- METODOLOGÍA DE ESTUDIO -->
    <div class="methodology-card">
        <h2>(⁠✦⁠ ω ✦⁠) Metodología de Estudio Autónoma (8 Pasos)</h2>
        <div class="method-grid">
            <div class="method-item"><strong>1. 🎯 Objetivo:</strong> Qué vas a dominar.</div>
            <div class="method-item"><strong>2. 📖 Conceptos clave:</strong> Términos esenciales.</div>
            <div class="method-item"><strong>3. 🧩 Paso a paso:</strong> Procedimiento resuelto.</div>
            <div class="method-item"><strong>4. ⚠️ Errores:</strong> Trampas a evitar.</div>
            <div class="method-item"><strong>5. ✏️ Práctica:</strong> Ejercicio autónomo.</div>
            <div class="method-item"><strong>6. 🔍 Comprobación:</strong> Verificación de sentido.</div>
            <div class="method-item"><strong>7. 🔗 Conexiones:</strong> Relación conceptual.</div>
            <div class="method-item"><strong>8. 🟢🟡🔴 Evaluación:</strong> Control de nivel.</div>
        </div>
    </div>

    <!-- ==================== FÍSICA ==================== -->
    <h2 class="subject-header" style="color: #d64550;">⚡ Física</h2>

    <!-- Física y Medición / Vectores -->
    <div class="kawaii-card">
        <span class="badge badge-reconocer">🟢 RECONOCER</span>
        <h3>Medición, Escalares y Vectores</h3>
        
        <div class="step-block">
            <span class="step-label">1. 🎯 Objetivo:</span> Diferenciar magnitudes escalares de vectoriales y operar con componentes trigonométricas ($x = M \cdot \cos\theta$, $y = M \cdot \sin\theta$).
        </div>

        <div class="step-block">
            <span class="step-label">2. 📖 Conceptos clave:</span> Unidades SI, Escalar (magnitud sola), Vectorial (magnitud + dirección), Componentes rectangulares.
        </div>

        <div class="example-box">
            <span class="step-label">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><strong>Problema:</strong> Un vector fuerza $F = 10\text{ N}$ se aplica a un ángulo de $30^\circ$. Hallar sus componentes.</p>
            <ul>
                <li><strong>Componente X:</strong> $F_x = 10 \cdot \cos(30^\circ) = 10 \cdot 0.866 = 8.66\text{ N}$</li>
                <li><strong>Componente Y:</strong> $F_y = 10 \cdot \sin(30^\circ) = 10 \cdot 0.5 = 5.0\text{ N}$</li>
            </ul>
        </div>

        <div class="synoptic-box">
            <strong>Cuadro Sinóptico</strong>
            <ul>
                <li><strong>Escalar:</strong> Mide solo magnitud (ej: Masa $kg$, Tiempo $s$, Temperatura $^\circ C$).</li>
                <li><strong>Vectorial:</strong> Requiere dirección (ej: Fuerza $N$, Velocidad $m/s$).</li>
            </ul>
        </div>
    </div>

    <!-- Cinemática y Leyes de Newton -->
    <div class="kawaii-card">
        <span class="badge badge-resolver">🔴 RESOLVER</span>
        <h3>Cinemática (MRU / MRUV) y Leyes de Newton</h3>

        <div class="step-block">
            <span class="step-label">1. 🎯 Objetivo:</span> Calcular posiciones, velocidades y aceleraciones bajo fuerza constante ($F = m \cdot a$).
        </div>

        <div class="example-box">
            <span class="step-label">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><strong>Problema:</strong> Un carrito de $m = 2\text{ kg}$ acelera de $0$ a $20\text{ m/s}$ en $5\text{ s}$. Hallar la fuerza neta ejercida.</p>
            <ul>
                <li><strong>Aceleración:</strong> $a = \frac{v - v_0}{t} = \frac{20 - 0}{5} = 4\text{ m/s}^2$</li>
                <li><strong>Fuerza neta:</strong> $F = m \cdot a = 2\text{ kg} \cdot 4\text{ m/s}^2 = 8\text{ N}$</li>
            </ul>
        </div>

        <div class="warning-box">
            <strong>⚠️ Error frecuente:</strong> En gráficos $x$-$t$, la pendiente es la velocidad. En $v$-$t$, la pendiente es la aceleración y el área bajo la curva representa el desplazamiento.
        </div>

        <div class="synoptic-box">
            <strong>Leyes de Newton</strong>
            <ul>
                <li><strong>1ª Ley (Inercia):</strong> Estado uniforme sin fuerza externa.</li>
                <li><strong>2ª Ley:</strong> $F = m \cdot a$</li>
                <li><strong>3ª Ley:</strong> Acción y reacción iguales y opuestas.</li>
            </ul>
        </div>
    </div>

    <!-- Hidrostática -->
    <div class="kawaii-card">
        <span class="badge badge-resolver">🔴 RESOLVER</span>
        <h3>Hidrostática: Presión, Pascal y Arquímedes</h3>

        <div class="step-block">
            <span class="step-label">1. 🎯 Objetivo:</span> Calcular la presión absoluta a cierta profundidad y la fuerza de empuje sobre cuerpos sumergidos.
        </div>

        <div class="example-box">
            <span class="step-label">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><strong>Problema:</strong> Un buzo está a $h = 10\text{ m}$ en el mar ($\rho = 1025\text{ kg/m}^3$, $P_0 = 101325\text{ Pa}$). Calculá la presión absoluta.</p>
            <ul>
                <li><strong>Presión manométrica:</strong> $P_{man} = \rho \cdot g \cdot h = 1025 \cdot 9.8 \cdot 10 = 100450\text{ Pa}$</li>
                <li><strong>Presión absoluta:</strong> $P_{abs} = P_0 + P_{man} = 101325 + 100450 = 201775\text{ Pa} \approx 201.78\text{ kPa}$</li>
            </ul>
        </div>

        <div class="warning-box">
            <strong>⚠️ Error frecuente:</strong> No confundir la presión manométrica con la absoluta (que incluye la atmosférica $P_0$).
        </div>

        <div class="step-block">
            <span class="step-label">5. ✏️ Ejercicio autónomo:</span> Un objeto de $V = 0.02\text{ m}^3$ se sumerge en agua ($\rho = 1000\text{ kg/m}^3$). Calculá el empuje de Arquímedes ($E = \rho \cdot g \cdot V$).
        </div>

        <div class="step-block">
            <span class="step-label">7. 🔗 Conexión conceptual:</span> Presión hidrostática → Hidrodinámica → Presión sanguínea en biología.
        </div>

        <div class="synoptic-box">
            <strong>Hidrostática</strong>
            <ul>
                <li><strong>Ecuación de presión:</strong> $P = P_0 + \rho \cdot g \cdot h$</li>
                <li><strong>P. de Pascal:</strong> Presión aplicada a un fluido encerrado se transmite por igual.</li>
                <li><strong>P. de Arquímedes:</strong> Empuje es igual al peso del fluido desalojado.</li>
            </ul>
        </div>
    </div>

    <!-- Hidrodinámica y Viscosidad -->
    <div class="kawaii-card">
        <span class="badge badge-entender">🟡 ENTENDER</span>
        <h3>Hidrodinámica, Viscosidad y Difusión</h3>

        <p><strong>Continuidad:</strong> $A_1 v_1 = A_2 v_2$. Si el área del tubo se reduce, la velocidad del fluido aumenta.</p>
        <p><strong>Bernoulli:</strong> $P + \frac{1}{2}\rho v^2 + \rho g h = \text{cte}$. Cuando un fluido circula por un conducto que se estrecha, su velocidad puede aumentar y, bajo ciertas condiciones, su presión disminuir.</p>
        <p><strong>Ley de Poiseuille:</strong> $Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$. El caudal depende fuertemente del radio $r$ elevado a la cuarta potencia.</p>
        
        <div class="warning-box">
            <strong>⚠️ Corrección científica importante (Ósmosis):</strong> El agua no desplaza su flujo buscando "igualar concentraciones" de forma consciente; se desplaza pasivamente a través de una membrana semipermeable hacia el lado con mayor concentración efectiva de solutos según las condiciones del sistema.
        </div>
    </div>

    <!-- ==================== QUÍMICA ==================== -->
    <h2 class="subject-header" style="color: #c86d3b;">🧪 Química</h2>

    <div class="kawaii-card">
        <span class="badge badge-entender">🟡 ENTENDER</span>
        <h3>Sustancias, Átomos y Estructura</h3>

        <div class="warning-box">
            <strong>⚠️ Correcciones científicas conceptuales:</strong>
            <ul>
                <li><strong>Sustancias puras:</strong> Las sustancias puras tienen composición constante. Las mezclas pueden separarse mediante métodos físicos; en cambio, un compuesto puede descomponerse en sustancias más simples mediante procesos químicos[cite: 1].</li>
                <li><strong>Átomo:</strong> Los electrones no orbitan en trayectorias rígidas; se ubican en una <em>nube electrónica / orbitales</em>[cite: 1].</li>
                <li><strong>Química Inorgánica:</strong> Estudia los compuestos que no se clasifican como orgánicos[cite: 1]. Incluye óxidos, ácidos, bases, sales y muchos otros compuestos[cite: 1].</li>
            </ul>
        </div>

        <p><strong>Tipos de Enlace:</strong></p>
        <ul>
            <li><strong>Iónico:</strong> Metal + No metal (transferencia de electrones).</li>
            <li><strong>Covalente:</strong> No metal + No metal (compartición de electrones).</li>
            <li><strong>Metálico:</strong> Red de cationes rodeados por mar de electrones.</li>
        </ul>
    </div>

    <div class="kawaii-card">
        <span class="badge badge-resolver">🔴 RESOLVER</span>
        <h3>Soluciones, Molaridad, pH y Estequiometría</h3>

        <div class="step-block">
            <span class="step-label">1. 🎯 Objetivo:</span> Balancear reacciones, hallar el reactivo limitante y calcular la molaridad ($M$) y el $pH$.
        </div>

        <div class="example-box">
            <span class="step-label">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><strong>Problema:</strong> Se disuelven $0.5\text{ moles}$ de $\text{HCl}$ en agua hasta completar $2\text{ litros}$ de solución. Calculá Molaridad y $pH$.</p>
            <ul>
                <li><strong>Molaridad:</strong> $M = \frac{\text{moles de soluto}}{\text{litros de solución}} = \frac{0.5}{2} = 0.25\text{ M}$</li>
                <li><strong>Cálculo de pH:</strong> $pH = -\log[H^+] = -\log(0.25) \approx 0.60$</li>
            </ul>
        </div>

        <div class="synoptic-box">
            <strong>Fórmulas Básicas</strong>
            <ul>
                <li><strong>Número de Avogadro:</strong> $1\text{ mol} = 6.022 \times 10^{23}\text{ partículas}$</li>
                <li><strong>Dilución:</strong> $C_1 \cdot V_1 = C_2 \cdot V_2$</li>
                <li><strong>Redox:</strong> Oxidación (pérdida de $e^-$), Reducción (ganancia de $e^-$).</li>
            </ul>
        </div>
    </div>

    <!-- ==================== BIOLOGÍA ==================== -->
    <h2 class="subject-header" style="color: #2e7d6e;">🧬 Biología</h2>

    <div class="kawaii-card">
        <span class="badge badge-entender">🟡 ENTENDER</span>
        <h3>Célula, Genética, Mutación y Evolución</h3>

        <div class="warning-box">
            <strong>⚠️ Correcciones científicas aplicadas:</strong>
            <ul>
                <li><strong>Genoma:</strong> Todo el material genético de un organismo, incluidos los genes y otras regiones de ADN[cite: 1].</li>
                <li><strong>Gen:</strong> Segmento de ADN que contiene información para producir un producto funcional, como una proteína o un ARN[cite: 1].</li>
                <li><strong>Evolución / Selección natural:</strong> Ciertas variantes se vuelven más frecuentes cuando favorecen la supervivencia o reproducción en un ambiente determinado[cite: 1].</li>
                <li><strong>Respiración Celular:</strong> La célula obtiene ATP mediante la oxidación de nutrientes, como la glucosa[cite: 1]. En la respiración aeróbica suele utilizar oxígeno y liberar dióxido de carbono y agua[cite: 1] (Glucólisis, Ciclo de Krebs, Cadena respiratoria).</li>
                <li><strong>Meiosis:</strong> Genera gametos diferentes mediante la recombinación homóloga y la distribución independiente de los cromosomas (no crea variabilidad "entre padres e hijos" directamente)[cite: 1].</li>
            </ul>
        </div>

        <p><strong>Flujo de la Información Genética:</strong> Replicación ($\text{ADN} \to \text{ADN}$), Transcripción ($\text{ADN} \to \text{ARNm}$), Traducción ($\text{ARNm} \to \text{Proteína}$).</p>
    </div>

    <!-- ==================== MATEMÁTICA ==================== -->
    <h2 class="subject-header" style="color: #6c5ce7;">📐 Matemática</h2>

    <div class="kawaii-card">
        <span class="badge badge-resolver">🔴 RESOLVER</span>
        <h3>Álgebra, Cálculo y Grafos</h3>

        <div class="warning-box">
            <strong>⚠️ Aclaración importante:</strong> En problemas de Regla de tres simple, debe aclararse o comprobarse previamente que la relación sea de estricta proporcionalidad[cite: 1].
        </div>

        <p><strong>Representación geométrica fundamental:</strong></p>
        <ul>
            <li><strong>Derivada:</strong> Representa la pendiente de la recta tangente a la curva o la tasa de cambio instantánea.</li>
            <li><strong>Integral:</strong> Representa el área acumulada bajo la curva entre dos puntos.</li>
        </ul>

        <div class="synoptic-box">
            <strong>Cuadro Sinóptico</strong>
            <ul>
                <li><strong>Álgebra Lineal:</strong> Vectores (listas de números) y Matrices (tablas). Base para PCA y reducción de dimensiones.</li>
                <li><strong>Grafos:</strong> Nodos (elementos) y Aristas (conexiones). Modelan redes biológicas o metabólicas.</li>
            </ul>
        </div>
    </div>

    <!-- ==================== PROGRAMACIÓN ==================== -->
    <h2 class="subject-header" style="color: #4a4e69;">💻 Programación (Python)</h2>

    <div class="kawaii-card">
        <span class="badge badge-resolver">🔴 RESOLVER</span>
        <h3>Estructuras, Búsqueda y Manejo de Datos</h3>

        <div class="step-block">
            <span class="step-label">Patrón 1: Frecuencia de caracteres en un string</span>
            <div class="code-container">
secuencia = "ATGCGTAC"
conteo = {}

for base in secuencia:
    conteo[base] = conteo.get(base, 0) + 1

print(conteo)  # {'A': 2, 'T': 2, 'G': 2, 'C': 2}
            </div>
        </div>

        <div class="step-block">
            <span class="step-label">Patrón 2: Lectura segura de archivos con `with open`</span>
            <div class="code-container">
with open("secuencia.txt") as archivo:
    contenido = archivo.read()
    print(contenido)
            </div>
        </div>

        <div class="warning-box">
            <strong>⚠️ Corrección sobre búsqueda y ordenamiento:</strong> Ordenar los datos no hace más rápida la búsqueda por sí mismo; lo que hace es permitir el uso de métodos de búsqueda mucho más eficientes, como la <em>búsqueda binaria</em> ($O(\log n)$)[cite: 1].
        </div>
    </div>

    <!-- ==================== FORMULARIO UNIFICADO ==================== -->
    <h2 class="subject-header" style="color: #9a8c98;">📑 Formulario Unificado & Constantes</h2>

    <table>
        <thead>
            <tr>
                <th>Materia</th>
                <th>Concepto / Magnitud</th>
                <th>Fórmula / Valor</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Física</strong></td>
                <td>Aceleración de Gravedad ($g$)</td>
                <td>$g \approx 9.8\text{ m/s}^2$</td>
            </tr>
            <tr>
                <td><strong>Física</strong></td>
                <td>Presión Hidrostática / Absoluta</td>
                <td>$P = P_0 + \rho \cdot g \cdot h$</td>
            </tr>
            <tr>
                <td><strong>Física</strong></td>
                <td>Ley de Poiseuille (Caudal)</td>
                <td>$Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$</td>
            </tr>
            <tr>
                <td><strong>Química</strong></td>
                <td>Número de Avogadro ($N_A$)</td>
                <td>$6.022 \times 10^{23}\text{ mol}^{-1}$</td>
            </tr>
            <tr>
                <td><strong>Química</strong></td>
                <td>Molaridad / pH</td>
                <td>$M = \frac{n}{V(\text{L})}, \quad pH = -\log[H^+]$</td>
            </tr>
            <tr>
                <td><strong>Matemática</strong></td>
                <td>Resolvente Cuadrática</td>
                <td>$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$</td>
            </tr>
        </tbody>
    </table>

</div>

</body>
</html>
