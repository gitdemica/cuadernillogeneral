<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cuadernillo de Estudio Integral - Ciencias Exactas y Programación</title>
    <!-- MathJax para renderizado de fórmulas matemáticas LaTeX -->
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --bg-light: #f8f9fa;
            --border-color: #e9ecef;
            --text: #2d3748;
            --green: #2ecc71;
            --yellow: #f1c40f;
            --red: #e74c3c;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: #f4f6f8;
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: #ffffff;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        h1, h2, h3, h4 {
            color: var(--primary);
            font-weight: 700;
        }

        h1 {
            border-bottom: 3px solid var(--secondary);
            padding-bottom: 10px;
            margin-top: 0;
        }

        h2 {
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 8px;
            margin-top: 40px;
        }

        .level-badge {
            display: inline-block;
            padding: 4px 8px;
            border-radius: 4px;
            font-weight: bold;
            font-size: 0.85em;
            margin-bottom: 10px;
        }
        .level-reconocer { background-color: #e8f8f5; color: #117a65; }
        .level-entender { background-color: #fef9e7; color: #b7950b; }
        .level-resolver { background-color: #fadbd8; color: #78281f; }

        .pedagogical-block {
            background-color: #ffffff;
            border: 1px solid var(--border-color);
            border-left: 4px solid var(--secondary);
            border-radius: 4px;
            padding: 20px;
            margin-bottom: 30px;
        }

        .pedagogical-step {
            margin-bottom: 12px;
        }

        .pedagogical-step-title {
            font-weight: bold;
            color: var(--primary);
        }

        .warning-box {
            background-color: #fdf2e9;
            border-left: 4px solid #e67e22;
            padding: 10px 15px;
            margin: 10px 0;
            border-radius: 0 4px 4px 0;
        }

        .code-block {
            background-color: #272822;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 5px;
            font-family: "Courier New", Courier, monospace;
            overflow-x: auto;
            margin: 10px 0;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        th, td {
            border: 1px solid var(--border-color);
            padding: 10px;
            text-align: left;
        }

        th {
            background-color: var(--bg-light);
            color: var(--primary);
        }

        .synoptic-box {
            background-color: var(--bg-light);
            border: 1px dashed var(--secondary);
            padding: 15px;
            border-radius: 5px;
            margin-top: 15px;
        }

        @media print {
            body { background: white; padding: 0; }
            .container { box-shadow: none; padding: 0; max-width: 100%; }
            .pedagogical-block { page-break-inside: avoid; }
            h2 { page-break-before: always; }
        }
    </style>
</head>
<body>

<div class="container">

    <section>
        <h2>¿Cómo estudiar con este documento?</h2>
        <p>Este material está estructurado bajo una secuencia de 8 pasos para garantizar el aprendizaje autónomo e integrador:</p>
        <ol>
            <li><strong>🎯 Objetivo del tema:</strong> Qué habilidad concreta vas a dominar.</li>
            <li><strong>📖 Conceptos clave:</strong> Términos fundamentales de reconocimiento inmediato.</li>
            <li><strong>🧩 Ejemplo resuelto paso a paso:</strong> Procedimiento detallado (Datos → Método → Desarrollo → Resultado).</li>
            <li><strong>⚠️ Errores frecuentes:</strong> Trampas conceptuales comunes que debés evitar.</li>
            <li><strong>✏️ Ejercicio práctico:</strong> Problema para resolver sin asistencia inmediata.</li>
            <li><strong>🔍 Verificación:</strong> Métodos de comprobación de coherencia de la respuesta.</li>
            <li><strong>🔗 Conexión conceptual:</strong> Relación directa con otras disciplinas.</li>
            <li><strong>🟢🟡🔴 Autoevaluación:</strong> Nivel de control adquirido (Reconocer / Entender / Resolver).</li>
        </ol>
    </section>

    <!-- ==================== FÍSICA ==================== -->
    <h2>Física</h2>

    <div class="pedagogical-block">
        <span class="level-badge level-resolver">🔴 RESOLVER</span>
        <h3>Hidrostática: Presión, Pascal y Arquímedes</h3>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">1. 🎯 Objetivo:</span> Calcular la presión absoluta a distintas profundidades y la fuerza de empuje sobre cuerpos sumergidos.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">2. 📖 Conceptos clave:</span> Presión hidrostática, Presión absoluta, Principio de Pascal, Empuje, Arquímedes.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><em>Problema:</em> Un buzo se encuentra a $10\text{ m}$ de profundidad en el mar ($\rho = 1025\text{ kg/m}^3$). La presión atmosférica en la superficie es $P_0 = 101325\text{ Pa}$. Calculá la presión absoluta que soporta.</p>
            <ul>
                <li><strong>Datos:</strong> $P_0 = 101325\text{ Pa}$, $\rho = 1025\text{ kg/m}^3$, $g = 9.8\text{ m/s}^2$, $h = 10\text{ m}$.</li>
                <li><strong>Método:</strong> Aplicar la ecuación fundamental de la hidrostática $P = P_0 + \rho \cdot g \cdot h$.</li>
                <li><strong>Procedimiento:</strong>
                    <br> $P_{manometrica} = 1025\text{ kg/m}^3 \cdot 9.8\text{ m/s}^2 \cdot 10\text{ m} = 100450\text{ Pa}$
                    <br> $P_{absoluta} = 101325\text{ Pa} + 100450\text{ Pa} = 201775\text{ Pa}$
                </li>
                <li><strong>Resultado:</strong> $P = 201.78\text{ kPa}$ (aproximadamente $2\text{ atm}$).</li>
            </ul>
        </div>

        <div class="warning-box">
            <strong>⚠️ Errores frecuentes:</strong> No confundir la presión manométrica ($\rho \cdot g \cdot h$) con la presión absoluta (que suma la presión atmosférica $P_0$).
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">5. ✏️ Ejercicio para hacer sola:</span> Un objeto de volumen $V = 0.02\text{ m}^3$ se sumerge completamente en agua ($\rho = 1000\text{ kg/m}^3$). Calculá el empuje que experimenta según el Principio de Arquímedes.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">6. 🔍 Verificación:</span> Comprobá que las unidades dimensionales se cancelen correctamente hasta obtener Newtons ($N = \text{kg}\cdot\text{m/s}^2$).
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">7. 🔗 Conexión con otros temas:</span> Presión hidrostática → Dinámica de fluidos → Transporte cardiovascular y presión sanguínea.
        </div>

        <div class="synoptic-box">
            <strong>Cuadro sinóptico - Hidrostática</strong>
            <ul>
                <li><strong>Presión absoluta:</strong> $P = P_0 + \rho \cdot g \cdot h$</li>
                <li><strong>Principio de Pascal:</strong> Transmisión uniforme de presión en fluidos incompresibles.</li>
                <li><strong>Principio de Arquímedes:</strong> $E = \rho_{fluido} \cdot g \cdot V_{desalojado}$</li>
            </ul>
        </div>

        <div class="pedagogical-step" style="margin-top: 10px;">
            <span class="pedagogical-step-title">8. 🟢🟡🔴 Autoevaluación:</span>
            <span>🟢 Reconozco las fórmulas | 🟡 Puedo explicar Pascal y Arquímedes | 🔴 Resuelvo ejercicios numéricos sin ayuda</span>
        </div>
    </div>

    <div class="pedagogical-block">
        <span class="level-badge level-entender">🟡 ENTENDER</span>
        <h3>Hidrodinámica y Viscosidad</h3>
        <p><strong>Ecuación de Continuidad:</strong> $A_1 v_1 = A_2 v_2$. Si la sección disminuye, la velocidad aumenta.</p>
        <p><strong>Ecuación de Bernoulli:</strong> $P + \frac{1}{2}\rho v^2 + \rho g h = \text{cte}$. Cuando un fluido circula por un conducto que se estrecha, su velocidad puede aumentar y, bajo ciertas condiciones, su presión disminuir.</p>
        <p><strong>Ley de Poiseuille:</strong> $Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$. El caudal depende fuertemente del radio elevado a la cuarta potencia.</p>
        <p><strong>Ley de Fick (Difusión):</strong> $J = -D \cdot \frac{\Delta C}{\Delta x}$. El flujo es proporcional al gradiente de concentración.</p>
        <div class="warning-box">
            <strong>⚠️ Corrección conceptual:</strong> El agua en la ósmosis no "busca igualar concentraciones" de manera consciente; se desplaza pasivamente a través de una membrana semipermeable hacia el lado con mayor concentración efectiva de solutos debido a un gradiente de potencial químico.
        </div>
    </div>

    <!-- ==================== QUÍMICA ==================== -->
    <h2>Química</h2>

    <div class="pedagogical-block">
        <span class="level-badge level-entender">🟡 ENTENDER</span>
        <h3>Sustancias, Átomos y Estructura</h3>
        
        <p><strong>Sustancias puras y mezclas:</strong> Las sustancias puras tienen composición constante. Las mezclas pueden separarse mediante métodos físicos; en cambio, un compuesto puede descomponerse en sustancias más simples mediante procesos químicos.</p>
        
        <p><strong>Estructura atómica:</strong> El átomo posee protones y neutrones en su núcleo, mientras que los electrones se distribuyen externamente en una <em>nube electrónica / orbitales</em> (no en órbitas rígidas predecibles).</p>
        
        <p><strong>Química Inorgánica:</strong> Estudia los compuestos que no se clasifican como orgánicos. Incluye óxidos, ácidos, bases, sales y muchos otros compuestos.</p>
    </div>

    <div class="pedagogical-block">
        <span class="level-badge level-resolver">🔴 RESOLVER</span>
        <h3>Soluciones, Molaridad y pH</h3>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">1. 🎯 Objetivo:</span> Calcular molaridades de soluciones acuosas y determinar el nivel de acidez/basicidad mediante pH.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">2. 📖 Conceptos clave:</span> Soluto, Solvente, Molaridad ($M$), Dilución, $pH$.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">3. 🧩 Ejemplo resuelto paso a paso:</span>
            <p><em>Problema:</em> Se disuelven $0.5\text{ moles}$ de $\text{HCl}$ en agua hasta completar $2\text{ litros}$ de solución. Calculá la molaridad y el $pH$.</p>
            <ul>
                <li><strong>Datos:</strong> $n = 0.5\text{ moles}$, $V = 2\text{ L}$.</li>
                <li><strong>Método:</strong> $M = \frac{n}{V}$ y $pH = -\log[H^+]$.</li>
                <li><strong>Procedimiento:</strong>
                    <br> $M = \frac{0.5\text{ mol}}{2\text{ L}} = 0.25\text{ M}$
                    <br> $[H^+] = 0.25\text{ M} \implies pH = -\log(0.25) \approx 0.60$
                </li>
                <li><strong>Resultado:</strong> Molaridad $0.25\text{ M}$, $pH = 0.60$ (altamente ácido).</li>
            </ul>
        </div>

        <div class="warning-box">
            <strong>⚠️ Errores frecuentes:</strong> No confundir volumen de solvente con volumen total de la solución al calcular Molaridad.
        </div>

        <div class="synoptic-box">
            <strong>Cuadro sinóptico - Fisicoquímica de Soluciones</strong>
            <ul>
                <li><strong>Molaridad:</strong> $M = \text{moles de soluto} / \text{litros de solución}$</li>
                <li><strong>Dilución:</strong> $C_1 \cdot V_1 = C_2 \cdot V_2$</li>
                <li><strong>Escala de pH:</strong> $pH = -\log[H^+]$ ($pH < 7$ Ácido, $pH = 7$ Neutro, $pH > 7$ Básico)</li>
            </ul>
        </div>
    </div>

    <!-- ==================== BIOLOGÍA ==================== -->
    <h2>Biología</h2>

    <div class="pedagogical-block">
        <span class="level-badge level-entender">🟡 ENTENDER</span>
        <h3>Bases Moleculares y Genética</h3>

        <p><strong>Genoma:</strong> Todo el material genético de un organismo, incluidos los genes y otras regiones de ADN.</p>
        
        <p><strong>Gen:</strong> Segmento de ADN que contiene información para producir un producto funcional, como una proteína o un ARN.</p>

        <p><strong>Evolución y Selección Natural:</strong> La selección natural es el proceso mediante el cual ciertas variantes genéticas se vuelven más frecuentes en una población cuando favorecen la supervivencia o la reproducción en un ambiente determinado.</p>

        <p><strong>Respiración Celular:</strong> La célula obtiene ATP mediante la oxidación de nutrientes, como la glucosa. En la respiración aeróbica suele utilizar oxígeno y liberar dióxido de carbono y agua (pasando por Glucólisis, Ciclo de Krebs y Cadena respiratoria).</p>

        <p><strong>Variabilidad Genética:</strong> La meiosis genera gametos diferentes mediante la recombinación homóloga y la distribución independiente de los cromosomas (no crea variabilidad "entre padres e hijos" directamente, sino en las gametas que darán origen a la descendencia).</p>
    </div>

    <!-- ==================== MATEMÁTICA ==================== -->
    <h2>Matemática</h2>

    <div class="pedagogical-block">
        <span class="level-badge level-resolver">🔴 RESOLVER</span>
        <h3>Cálculo, Álgebra y Álgebra Lineal</h3>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">1. 🎯 Objetivo:</span> Interpretar geométricamente y calcular la derivada e integral básica de una función.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">2. 📖 Conceptos clave:</span> Límite, Derivada (recta tangente / tasa de cambio), Integral (área acumulada), Matriz, Vector.
        </div>

        <div class="warning-box">
            <strong>⚠️ Condición de aplicación:</strong> Al usar la regla de tres simple en modelos reales, hay que verificar primero que exista una relación rigurosamente proporcional entre las magnitudes evaluadas.
        </div>

        <div class="synoptic-box">
            <strong>Cuadro sinóptico - Herramientas Matemáticas</strong>
            <ul>
                <li><strong>Derivada:</strong> $f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$ (Pendiente de la recta tangente).</li>
                <li><strong>Integral definida:</strong> $\int_{a}^{b} f(x)dx$ (Área bajo la curva entre $a$ y $b$).</li>
                <li><strong>Álgebra Lineal:</strong> Vectores $v \in \mathbb{R}^n$, Matrices $A \in \mathbb{R}^{m \times n}$. Base del análisis multidimensional.</li>
            </ul>
        </div>
    </div>

    <!-- ==================== PROGRAMACIÓN ==================== -->
    <h2>Programación (Python)</h2>

    <div class="pedagogical-block">
        <span class="level-badge level-resolver">🔴 RESOLVER</span>
        <h3>Manejo de Estructuras y Archivos</h3>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">1. 🎯 Objetivo:</span> Procesar cadenas de texto o secuencias utilizando estructuras de datos y lectura de archivos.
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">2. 🧩 Patrón de código: Frecuencia de elementos</span>
            <div class="code-block">
secuencia = "ATGCGTAC"
conteo = {}

for base in secuencia:
    conteo[base] = conteo.get(base, 0) + 1

print(conteo)  # Muestra: {'A': 2, 'T': 2, 'G': 2, 'C': 2}
            </div>
        </div>

        <div class="pedagogical-step">
            <span class="pedagogical-step-title">3. 🧩 Lectura segura de archivos:</span>
            <div class="code-block">
with open("datos.csv", "r") as archivo:
    lineas = archivo.readlines()
    for linea in lineas:
        print(linea.strip())
            </div>
        </div>

        <div class="warning-box">
            <strong>⚠️ Precisión técnica sobre algoritmos:</strong> Ordenar los datos no acelera la búsqueda mágicamente por sí solo; lo que hace es habilitar el uso de métodos de búsqueda mucho más eficientes, como la <em>búsqueda binaria</em> ($O(\log n)$).
        </div>
    </div>

    <!-- ==================== FORMULARIO UNIFICADO ==================== -->
    <h2>Hoja de Constantes y Formulario Unificado</h2>

    <table>
        <thead>
            <tr>
                <th>Disciplina</th>
                <th>Concepto / Magnitud</th>
                <th>Fórmula / Valor Constante</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Física</strong></td>
                <td>Aceleración de la Gravedad ($g$)</td>
                <td>$g \approx 9.8\text{ m/s}^2$</td>
            </tr>
            <tr>
                <td><strong>Física</strong></td>
                <td>Presión Hidrostática / Absolute</td>
                <td>$P = P_0 + \rho \cdot g \cdot h$</td>
            </tr>
            <tr>
                <td><strong>Física</strong></td>
                <td>Ecuación de Continuidad</td>
                <td>$A_1 v_1 = A_2 v_2$</td>
            </tr>
            <tr>
                <td><strong>Física</strong></td>
                <td>Ecuación de Bernoulli</td>
                <td>$P + \frac{1}{2}\rho v^2 + \rho g h = \text{constante}$</td>
            </tr>
            <tr>
                <td><strong>Física / Biología</strong></td>
                <td>Ley de Poiseuille (Caudal)</td>
                <td>$Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$</td>
            </tr>
            <tr>
                <td><strong>Química</strong></td>
                <td>Número de Avogadro ($N_A$)</td>
                <td>$N_A = 6.022 \times 10^{23}\text{ partículas/mol}$</td>
            </tr>
            <tr>
                <td><strong>Química</strong></td>
                <td>Molaridad ($M$) / pH</td>
                <td>$M = \frac{n}{V(\text{L})}, \quad pH = -\log[H^+]$</td>
            </tr>
            <tr>
                <td><strong>Matemática</strong></td>
                <td>Ecuación Cuadrática (Resolvente)</td>
                <td>$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$</td>
            </tr>
        </tbody>
    </table>

</div>

</body>
</html>
