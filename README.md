<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cuadernillo de Estudio - Ciencias Exactas y Aplicadas</title>
    <!-- Fuentes modernas redondeadas -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@400;500;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
    <!-- MathJax para el renderizado de fórmulas LaTeX -->
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    
    <style>
        :root {
            --bg-page: #f8fafc;
            --card-bg: #ffffff;
            --text-dark: #334155;
            --text-muted: #64748b;
            --border-radius: 16px;
            --shadow-soft: 0 4px 20px -2px rgba(148, 163, 184, 0.15);

            /* Paleta de colores por materia */
            --color-quimica: #c2410c;
            --bg-quimica: #fff7ed;
            --border-quimica: #ffedd5;

            --color-fisica: #be123c;
            --bg-fisica: #fff1f2;
            --border-fisica: #ffe4e6;

            --color-biologia: #15803d;
            --bg-biologia: #f0fdf4;
            --border-biologia: #dcfce7;

            --color-matematica: #6b21a8;
            --bg-matematica: #faf5ff;
            --border-matematica: #f3e8ff;

            --color-programacion: #0369a1;
            --bg-programacion: #f0f9ff;
            --border-programacion: #e0f2fe;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { font-family: 'M PLUS Rounded 1c', sans-serif; background-color: var(--bg-page); color: var(--text-dark); line-height: 1.7; padding: 30px 15px; }
        .container { max-width: 940px; margin: 0 auto; }

        /* Estilos de encabezado y tarjetas generales */
        .subject-header { 
            font-size: 1.8rem; 
            font-weight: 800; 
            margin: 40px 0 20px 0; 
            padding: 12px 20px; 
            border-radius: 12px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .topic-card {
            background: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 28px;
            margin-bottom: 30px;
            box-shadow: var(--shadow-soft);
            border: 2px solid #e2e8f0;
        }

        .badge { display: inline-flex; padding: 4px 14px; border-radius: 50px; font-size: 0.8rem; font-weight: 700; margin-bottom: 15px; }
        .badge-reconocer { background: #e0f2fe; color: #0369a1; border: 1px solid #bae6fd; }
        .badge-entender { background: #fef3c7; color: #b45309; border: 1px solid #fde68a; }
        .badge-resolver { background: #ffe4e6; color: #be123c; border: 1px solid #fecdd3; }

        .section-title { font-weight: 700; color: #475569; margin-top: 14px; margin-bottom: 4px; display: flex; align-items: center; gap: 6px; }

        .example-box { background: #f8fafc; border-left: 4px solid #94a3b8; padding: 16px 20px; border-radius: 12px; margin: 16px 0; font-size: 0.95rem; }
        .practice-box { background: #f0fdf4; border-left: 4px solid #4ade80; padding: 16px 20px; border-radius: 12px; margin: 16px 0; font-size: 0.95rem; }
        .solution-box { background: #f8fafc; border: 1px solid #e2e8f0; padding: 14px 18px; border-radius: 12px; margin: 12px 0; font-size: 0.92rem; }
        .warning-box { background: #fffbebf5; border-left: 4px solid #fcd34d; padding: 14px 18px; border-radius: 12px; margin: 16px 0; font-size: 0.92rem; color: #92400e; }
        
        .synoptic-box { background: #f8fafc; border: 2px dashed #cbd5e1; padding: 16px 20px; border-radius: 14px; margin: 16px 0; font-size: 0.92rem; }
        .synoptic-box ul { list-style: none; padding-left: 0; }
        .synoptic-box li { position: relative; padding-left: 18px; margin-bottom: 6px; }
        .synoptic-box li::before { content: "✦"; position: absolute; left: 0; font-weight: bold; }

        /* Estilos diferenciados por materia */
        .module-quimica .subject-header { background-color: var(--bg-quimica); color: var(--color-quimica); border: 1px solid var(--border-quimica); }
        .module-quimica .topic-card { border-color: var(--border-quimica); }
        .module-quimica .example-box { border-left-color: var(--color-quimica); background-color: var(--bg-quimica); }
        .module-quimica .synoptic-box { border-color: var(--color-quimica); }
        .module-quimica .synoptic-box li::before { color: var(--color-quimica); }

        /* Estilos Tabla Periódica */
        .ptable-container { overflow-x: auto; margin: 25px 0; }
        .ptable { width: 100%; border-collapse: collapse; min-width: 700px; font-size: 0.82rem; text-align: center; }
        .ptable th, .ptable td { border: 1px solid #cbd5e1; padding: 6px 4px; }
        .ptable th { background-color: #f1f5f9; font-weight: 700; }
        .elem-metal { background-color: #e0f2fe; }
        .elem-alcali { background-color: #fef3c7; }
        .elem-nometal { background-color: #dcfce7; }
        .elem-gas { background-color: #f3e8ff; }
        .elem-metaloid { background-color: #ffedd5; }

        @media print {
            body { background-color: white; padding: 0; }
            .topic-card { box-shadow: none; page-break-inside: avoid; }
            .subject-header { page-break-before: always; }
        }
    </style>
</head>
<body>

<div class="container">

    <!-- ==================== BLOQUE 1: QUÍMICA ==================== -->
    <div class="module-quimica">
        <h2 class="subject-header">🧪 Química</h2>

        <!-- 1. Sistemas Materiales y Sustancias -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Sistemas Materiales y Sustancias Puras</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia cómo se clasifica la materia según sus fases visibles y la forma en que sus componentes se dividen o descomponen[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Sistema Homogéneo:</strong> Presenta 1 sola fase continua con propiedades uniformes[cite: 1].</p>
            <p>• <strong>Sistema Heterogéneo:</strong> Presenta 2 o más fases separadas por superficies de contacto (interfases)[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificación conceptual precisa:</strong> Las mezclas pueden separarse mediante métodos físicos; en cambio, los compuestos pueden descomponerse en sustancias más simples mediante procesos químicos[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Mezclas:</strong> Composición variable $\to$ Separables por métodos físicos (filtración, destilación)[cite: 1].</li>
                    <li><strong>Compuestos:</strong> Composición constante $\to$ Descomponibles por métodos químicos[cite: 1].</li>
                    <li><strong>Elementos:</strong> Sustancias fundamentales $\to$ No se descomponen químicamente[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Clasificar un recipiente que contiene agua líquida, cubos de hielo y arena en el fondo[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar concepto):</strong> Determinar la cantidad de fases (porciones homogéneas físicamente diferenciables)[cite: 1].</p>
                <p>• <strong>Paso 2 (Reconocer elementos):</strong> Fase 1: agua líquida, Fase 2: hielo sólido, Fase 3: arena sólida[cite: 1].</p>
                <p>• <strong>Paso 3 (Relacionar):</strong> Aunque el agua y el hielo son la misma sustancia ($H_2O$), están en estados distintos, formando 2 fases diferentes[cite: 1].</p>
                <p>• <strong>Paso 4 (Explicar conclusión):</strong> Es un sistema heterogéneo formado por 3 fases y 2 componentes ($H_2O$ y arena)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Un sistema contiene agua completamente saturada de sal con cristales de sal depositados en el fondo. Indicar número de fases y componentes[cite: 1].</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Posee 2 fases (fase líquida salada + fase sólida de cristales de sal) y 2 componentes (agua y sal)[cite: 1].
            </div>
        </div>

        <!-- 2. Átomos y Estructura Atómica -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Átomos, Estructura Atómica y Tabla Periódica</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Describe la organización interna del átomo y el ordenamiento de los elementos en la Tabla Periódica[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Número Atómico ($Z$):</strong> Cantidad de protones en el núcleo; define la identidad del elemento[cite: 1].</p>
            <p>• <strong>Tabla Periódica:</strong> Ordena los elementos en grupos (columnas) y períodos (filas) según su número atómico[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificación conceptual precisa:</strong> El electrón posee carga negativa y se encuentra distribuido en la <em>nube electrónica / orbitales atómicos</em> (superando el concepto de órbita circular plana)[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Núcleo:</strong> Protones (carga $+$) + Neutrones (sin carga)[cite: 1].</li>
                    <li><strong>Electrón:</strong> Nube electrónica / orbitales (carga $-$)[cite: 1].</li>
                    <li><strong>Grupos / Períodos:</strong> Elementos del mismo grupo poseen propiedades químicas relacionadas[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Determinar la cantidad de subpartículas de un átomo neutro de Sodio ($Na$) con $Z = 11$ y Número Másico $A = 23$[cite: 1].</p>
                <p>• <strong>Paso 1:</strong> Identificar que $Z = \text{protones}$. Por lo tanto, tiene 11 protones[cite: 1].</p>
                <p>• <strong>Paso 2:</strong> Al ser un átomo neutro, la cantidad de electrones iguala a los protones: 11 electrones[cite: 1].</p>
                <p>• <strong>Paso 3:</strong> Calcular neutrones mediante $A - Z$: $23 - 11 = 12$ neutrones[cite: 1].</p>
                <p>• <strong>Resultado:</strong> 11 protones, 11 electrones en la nube electrónica y 12 neutrones[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Un átomo neutro de Carbono posee $Z = 6$ y $A = 12$. Indicar cuántos electrones orbitan en su nube electrónica y cuántos neutrones posee en su núcleo[cite: 1].</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Posee 6 electrones en su nube electrónica y 6 neutrones ($12 - 6 = 6$)[cite: 1].
            </div>
        </div>

        <!-- 3. Enlace Químico y Nomenclatura -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Enlace Químico, Química Inorgánica y Sales</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia cómo los átomos se unen para alcanzar estabilidad y cómo se forman y nombran las sustancias inorgánicas[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Enlace Iónico:</strong> Metal + No metal (transferencia de electrones)[cite: 1].</p>
            <p>• <strong>Enlace Covalente:</strong> No metal + No metal (compartición de electrones)[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificaciones conceptuales precisas:</strong>
                <br>• <strong>Química inorgánica:</strong> Estudia los compuestos que no se clasifican como orgánicos[cite: 1].
                <br>• <strong>Sales:</strong> Son compuestos iónicos; muchas de ellas se forman a partir de reacciones de neutralización ácido-base[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Iónico:</strong> Formación de cationes ($+$) y aniones ($-$)[cite: 1].</li>
                    <li><strong>Covalente:</strong> Formación de moléculas por pares compartidos[cite: 1].</li>
                    <li><strong>Sales:</strong> Compuestos iónicos formados comúnmente por un catión metálico y un anión no metálico[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Explicar el tipo de enlace en el Fluoruro de Litio ($LiF$)[cite: 1].</p>
                <p>• <strong>Paso 1:</strong> Identificar los elementos: Litio ($Li$, metal alcalino) y Flúor ($F$, no metal halógeno)[cite: 1].</p>
                <p>• <strong>Paso 2:</strong> Analizar la interacción: el Litio cede 1 electrón formando $Li^+$; el Flúor acepta ese electrón formando $F^-$[cite: 1].</p>
                <p>• <strong>Paso 3:</strong> Conclusión: Unión electrostática entre cationes y aniones $\to$ Enlace Iónico[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar qué tipo de enlace predomina en la molécula de agua ($H_2O$) sabiendo que el Hidrógeno y el Oxígeno son no metales[cite: 1].</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Enlace Covalente, ya que ambos no metales comparten electrones[cite: 1].
            </div>
        </div>

        <!-- 4. Mol, Masa Molar y Conversiones -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Mol, Masa Molar y Conversiones</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Permite vincular la escala microscópica de átomos y moléculas con las masas medibles en laboratorio[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Mol:</strong> Cantidad de sustancia que contiene $6.022 \times 10^{23}$ partículas elementales (Número de Avogadro)[cite: 1].</p>
            <p>• <strong>Masa Molar ($M$):</strong> Masa en gramos de 1 mol de sustancia ($g/mol$)[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Conversión:</strong> $\text{Moles } (n) = \frac{\text{Masa en gramos } (m)}{\text{Masa Molar } (M)}$[cite: 1].</li>
                    <li><strong>Partículas:</strong> $\text{Número de partículas} = n \times 6.022 \times 10^{23}$[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Calcular cuántos moles y cuántas moléculas hay en $36\text{ g}$ de agua ($H_2O$)[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar datos):</strong> $m = 36\text{ g}$. Masas atómicas: $H = 1\text{ g/mol}$, $O = 16\text{ g/mol}$[cite: 1].</p>
                <p>• <strong>Paso 2 (Elegir fórmula):</strong> $M_{H_2O} = (2 \times 1) + 16 = 18\text{ g/mol}$. Luego $n = m / M$[cite: 1].</p>
                <p>• <strong>Paso 3 (Reemplazar y aplicar):</strong> $n = 36\text{ g} / 18\text{ g/mol} = 2\text{ moles}$[cite: 1].</p>
                <p>• <strong>Paso 4 (Resolver moléculas):</strong> $2\text{ moles} \times 6.022 \times 10^{23} = 1.2044 \times 10^{24}\text{ moléculas}$[cite: 1].</p>
                <p>• <strong>Resultado:</strong> $2\text{ moles}$ que equivalen a $1.2044 \times 10^{24}\text{ moléculas}$[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Calcular la cantidad de moles presentes en $88\text{ g}$ de dióxido de carbono ($CO_2$). (Masas atómicas: $C = 12\text{ g/mol}$, $O = 16\text{ g/mol}$)[cite: 1].</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $M_{CO_2} = 12 + (2 \times 16) = 44\text{ g/mol}$. Moles $= 88\text{ g} / 44\text{ g/mol} = 2\text{ moles}$[cite: 1].
            </div>
        </div>

        <!-- 5. Soluciones y pH -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Soluciones, Molaridad y pH</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia la cuantificación de concentraciones de solutos disueltos en líquidos y la medida de acidez[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Molaridad ($M$):</strong> $M = \frac{\text{moles de soluto}}{\text{litros de solución}}$[cite: 1].</p>
            <p>• <strong>Escala de pH:</strong> $pH = -\log[H^+]$[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Molaridad:</strong> Unidades expresadas estrictamente en Moles por Litro ($mol/L$)[cite: 1].</li>
                    <li><strong>pH:</strong> Medida logarítmica ( $pH < 7$ Ácido | $pH = 7$ Neutro | $pH > 7$ Básico )[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Se disuelven $0.5\text{ moles}$ de $HCl$ en agua hasta alcanzar $2\text{ litros}$ de solución. Hallar Molaridad y $pH$[cite: 1].</p>
                <p>• <strong>Paso 1 (Datos):</strong> $n = 0.5\text{ mol}$, $V = 2\text{ L}$[cite: 1].</p>
                <p>• <strong>Paso 2 (Aplicar Molaridad):</strong> $M = 0.5\text{ mol} / 2\text{ L} = 0.25\text{ M}$[cite: 1].</p>
                <p>• <strong>Paso 3 (Aplicar pH):</strong> $[H^+] = 0.25\text{ M} \implies pH = -\log(0.25)$[cite: 1].</p>
                <p>• <strong>Paso 4 (Resolver):</strong> $pH = 0.60$[cite: 1].</p>
                <p>• <strong>Resultado:</strong> Solución $0.25\text{ M}$ con $pH = 0.60$ (altamente ácida)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Se preparan $500\text{ mL}$ ($0.5\text{ L}$) de solución disolviendo $0.1\text{ moles}$ de un ácido fuerte. Calculá su Molaridad[cite: 1].</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $M = 0.1\text{ mol} / 0.5\text{ L} = 0.2\text{ M}$[cite: 1].
            </div>
        </div>

        <!-- TABLA PERIÓDICA COMPLETA DE CONSULTA -->
        <div class="topic-card">
            <h3>🧪 Tabla Periódica de los Elementos (Herramienta de Consulta)</h3>
            
            <p style="font-size: 0.9rem; margin-top: 8px;">
                <strong>Guía rápida de uso:</strong>
                <br>• <strong>$Z$ (Número Atómico):</strong> Cantidad de protones en el núcleo.
                <br>• <strong>Período (Fila):</strong> Indica el número de niveles energéticos de los electrones.
                <br>• <strong>Grupo (Columna):</strong> Elementos del mismo grupo poseen propiedades químicas similares.
                <br>• <em>Herramienta de consulta continua: no es necesario memorizarla entera.</em>
            </p>

            <div class="ptable-container">
                <table class="ptable">
                    <thead>
                        <tr>
                            <th>Grupo</th>
                            <th>1</th><th>2</th><th>3-12</th><th>13</th><th>14</th><th>15</th><th>16</th><th>17</th><th>18</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>Período 1</strong></td>
                            <td class="elem-nometal">1<br><strong>H</strong><br>Hidrógeno</td>
                            <td colspan="7"></td>
                            <td class="elem-gas">2<br><strong>He</strong><br>Helio</td>
                        </tr>
                        <tr>
                            <td><strong>Período 2</strong></td>
                            <td class="elem-alcali">3<br><strong>Li</strong><br>Litio</td>
                            <td class="elem-metal">4<br><strong>Be</strong><br>Berilio</td>
                            <td class="elem-metal">Transición</td>
                            <td class="elem-metaloid">5<br><strong>B</strong><br>Boro</td>
                            <td class="elem-nometal">6<br><strong>C</strong><br>Carbono</td>
                            <td class="elem-nometal">7<br><strong>N</strong><br>Nitrógeno</td>
                            <td class="elem-nometal">8<br><strong>O</strong><br>Oxígeno</td>
                            <td class="elem-nometal">9<br><strong>F</strong><br>Flúor</td>
                            <td class="elem-gas">10<br><strong>Ne</strong><br>Neón</td>
                        </tr>
                        <tr>
                            <td><strong>Período 3</strong></td>
                            <td class="elem-alcali">11<br><strong>Na</strong><br>Sodio</td>
                            <td class="elem-metal">12<br><strong>Mg</strong><br>Magnesio</td>
                            <td class="elem-metal">Transición</td>
                            <td class="elem-metal">13<br><strong>Al</strong><br>Aluminio</td>
                            <td class="elem-metaloid">14<br><strong>Si</strong><br>Silicio</td>
                            <td class="elem-nometal">15<br><strong>P</strong><br>Fósforo</td>
                            <td class="elem-nometal">16<br><strong>S</strong><br>Azufre</td>
                            <td class="elem-nometal">17<br><strong>Cl</strong><br>Cloro</td>
                            <td class="elem-gas">18<br><strong>Ar</strong><br>Argón</td>
                        </tr>
                        <tr>
                            <td><strong>Período 4</strong></td>
                            <td class="elem-alcali">19<br><strong>K</strong><br>Potasio</td>
                            <td class="elem-metal">20<br><strong>Ca</strong><br>Calcio</td>
                            <td class="elem-metal">21-30<br>Fe, Cu, Zn...</td>
                            <td class="elem-metal">31<br><strong>Ga</strong><br>Galio</td>
                            <td class="elem-metaloid">32<br><strong>Ge</strong><br>Germanio</td>
                            <td class="elem-metaloid">33<br><strong>As</strong><br>Arsénico</td>
                            <td class="elem-nometal">34<br><strong>Se</strong><br>Selenio</td>
                            <td class="elem-nometal">35<br><strong>Br</strong><br>Bromo</td>
                            <td class="elem-gas">36<br><strong>Kr</strong><br>Kriptón</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <p style="font-size: 0.8rem; color: var(--text-muted); text-align: center;">
                <strong>Leyenda:</strong> 
                <span style="background:#fef3c7; padding:2px 6px; border-radius:4px;">Alcalinos</span> | 
                <span style="background:#e0f2fe; padding:2px 6px; border-radius:4px;">Metales</span> | 
                <span style="background:#ffedd5; padding:2px 6px; border-radius:4px;">Metaloides</span> | 
                <span style="background:#dcfce7; padding:2px 6px; border-radius:4px;">No Metales</span> | 
                <span style="background:#f3e8ff; padding:2px 6px; border-radius:4px;">Gases Nobles</span>
            </p>
        </div>
    </div>

/* Estilos específicos para Física */
        .module-fisica .subject-header { background-color: var(--bg-fisica); color: var(--color-fisica); border: 1px solid var(--border-fisica); }
        .module-fisica .topic-card { border-color: var(--border-fisica); }
        .module-fisica .example-box { border-left-color: var(--color-fisica); background-color: var(--bg-fisica); }
        .module-fisica .synoptic-box { border-color: var(--color-fisica); }
        .module-fisica .synoptic-box li::before { color: var(--color-fisica); }
        <!-- ==================== BLOQUE 2: FÍSICA ==================== -->
    <div class="module-fisica">
        <h2 class="subject-header">⚡ Física</h2>

        <!-- 1. Física y Medición -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Física y Medición</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia las magnitudes físicas y las unidades estandarizadas del Sistema Internacional (SI) para cuantificar fenómenos naturales[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Magnitudes Fundamentales:</strong> Longitud ($m$), Masa ($kg$), Tiempo ($s$)[cite: 1].</p>
            <p>• <strong>Magnitudes Derivadas:</strong> Resultan de combinar las fundamentales (ej: Velocidad en $m/s$, Fuerza en $N$)[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Sistema Internacional (SI):</strong> Base unificada de medición ($m, kg, s$)[cite: 1].</li>
                    <li><strong>Análisis Dimensional:</strong> Comprobación de consistencia de unidades en ambos lados de una igualdad[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Verificar si la unidad de la velocidad ($v = d / t$) es consistente[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar el concepto):</strong> La velocidad resulta del cociente entre distancia y tiempo[cite: 1].</p>
                <p>• <strong>Paso 2 (Reconocer elementos):</strong> La distancia se mide en metros ($m$) y el tiempo en segundos ($s$)[cite: 1].</p>
                <p>• <strong>Paso 3 (Relacionar):</strong> $\text{Unidad de } v = \frac{\text{metros}}{\text{segundos}} = \text{m/s}$[cite: 1].</p>
                <p>• <strong>Paso 4 (Explicar conclusión):</strong> La unidad $m/s$ es dimensionalmente válida. Si en un cálculo de velocidad obtienes $kg/s$, hay un error previo[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Sabiendo que la densidad se define como $\rho = m / V$, expresá sus unidades en el Sistema Internacional.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> La masa se mide en $kg$ y el volumen en $m^3$; por lo tanto, la unidad es $kg/m^3$.
            </div>
        </div>

        <!-- 2. Escalares, Vectores y Trigonometría -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Magnitudes Escalares, Vectoriales y Trigonometría</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Representa magnitudes físicas que poseen magnitud, dirección y sentido mediante vectores y trigonometría[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Escalar:</strong> Magnitud representada solo por un número y su unidad (temperatura, masa)[cite: 1].</p>
            <p>• <strong>Vectorial:</strong> Requiere magnitud, dirección y sentido (fuerza, velocidad)[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Componente X:</strong> $v_x = M \cdot \cos\theta$[cite: 1].</li>
                    <li><strong>Componente Y:</strong> $v_y = M \cdot \sin\theta$[cite: 1].</li>
                    <li><strong>Módulo:</strong> $M = \sqrt{v_x^2 + v_y^2}$.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Hallar las componentes del vector fuerza $F = 10\text{ N}$ que actúa a $\theta = 30^\circ$ sobre la horizontal[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar datos):</strong> Módulo $M = 10\text{ N}$, ángulo $\theta = 30^\circ$[cite: 1].</p>
                <p>• <strong>Paso 2 (Elegir fórmulas):</strong> $F_x = M \cdot \cos(30^\circ)$ y $F_y = M \cdot \sin(30^\circ)$[cite: 1].</p>
                <p>• <strong>Paso 3 (Reemplazar y calcular):</strong>
                    <br>$F_x = 10 \cdot 0.866 = 8.66\text{ N}$[cite: 1]
                    <br>$F_y = 10 \cdot 0.5 = 5.0\text{ N}$[cite: 1]
                </p>
                <p>• <strong>Paso 4 (Resultado):</strong> El vector expresado en componentes es $(8.66\text{ N}, 5.0\text{ N})$[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Calculá la componente horizontal $v_x$ de una velocidad de $20\text{ m/s}$ inclinada a $60^\circ$ respecto a la horizontal.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $v_x = 20 \cdot \cos(60^\circ) = 20 \cdot 0.5 = 10\text{ m/s}$.
            </div>
        </div>

        <!-- 3. Cinemática Básica -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Cinemática Básica (MRU y MRUV)</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Describe el movimiento de los cuerpos en función del tiempo sin considerar las causas que lo producen[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>MRU:</strong> Velocidad constante ($a = 0$). Fórmula: $x = x_0 + v \cdot t$[cite: 1].</p>
            <p>• <strong>MRUV:</strong> Aceleración constante ($a \neq 0$). Fórmula: $v = v_0 + a \cdot t$ y $x = x_0 + v_0 t + \frac{1}{2}a t^2$[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Interpretación gráfica:</strong> En un gráfico posición-tiempo ($x$-$t$), la pendiente es la velocidad; en un gráfico velocidad-tiempo ($v$-$t$), la pendiente representa la aceleración y el área bajo la curva es el desplazamiento[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>MRU:</strong> $v = \text{constante} \quad | \quad x = x_0 + v \cdot t$[cite: 1].</li>
                    <li><strong>MRUV:</strong> $a = \text{constante} \quad | \quad v = v_0 + a \cdot t \quad | \quad x = x_0 + v_0 t + \frac{1}{2}a t^2$[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Un móvil parte del reposo ($v_0 = 0$) y alcanza una velocidad de $20\text{ m/s}$ en $5\text{ s}$. Calcular su aceleración[cite: 1].</p>
                <p>• <strong>Paso 1 (Datos):</strong> $v_0 = 0\text{ m/s}$, $v = 20\text{ m/s}$, $t = 5\text{ s}$[cite: 1].</p>
                <p>• <strong>Paso 2 (Fórmula):</strong> $a = \frac{v - v_0}{t}$[cite: 1].</p>
                <p>• <strong>Paso 3 (Reemplazar y resolver):</strong> $a = \frac{20 - 0}{5} = 4\text{ m/s}^2$[cite: 1].</p>
                <p>• <strong>Paso 4 (Resultado):</strong> La aceleración del móvil es de $4\text{ m/s}^2$[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Utilizando la aceleración calculada de $4\text{ m/s}^2$, calculá la distancia recorrida en esos $5\text{ s}$ partiendo del reposo.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $x = 0 + (0 \cdot 5) + \frac{1}{2}(4)(5^2) = \frac{1}{2}(4)(25) = 50\text{ m}$.
            </div>
        </div>

        <!-- 4. Leyes de Newton y Energía -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Leyes de Newton, Trabajo y Conservación de la Energía</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Explica la causa del movimiento mediante fuerzas y cuantifica la transferencia y conservación de la energía[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>2ª Ley de Newton:</strong> $F = m \cdot a$[cite: 1].</p>
            <p>• <strong>Trabajo ($W$):</strong> $W = F \cdot d \cdot \cos\theta$[cite: 1]. <strong>Potencia ($P$):</strong> $P = W / t$[cite: 1].</p>
            <p>• <strong>Conservación:</strong> Sin rozamiento, $E_{mecanica} = E_c + E_p = \text{constante}$[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Leyes de Newton:</strong> 1ª Inercia | 2ª $F = ma$ | 3ª Acción-Reacción[cite: 1].</li>
                    <li><strong>Energía Cinética / Potencial:</strong> $E_c = \frac{1}{2}m v^2$ | $E_p = m \cdot g \cdot h$[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Calcular la energía potencial gravitatoria de un objeto de $1\text{ kg}$ situado a $5\text{ m}$ de altura ($g = 9.8\text{ m/s}^2$)[cite: 1].</p>
                <p>• <strong>Paso 1 (Datos):</strong> $m = 1\text{ kg}$, $g = 9.8\text{ m/s}^2$, $h = 5\text{ m}$[cite: 1].</p>
                <p>• <strong>Paso 2 (Fórmula):</strong> $E_p = m \cdot g \cdot h$[cite: 1].</p>
                <p>• <strong>Paso 3 (Resolver):</strong> $E_p = 1 \cdot 9.8 \cdot 5 = 49\text{ Joules}$[cite: 1].</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> Al caer al suelo sin fricción, toda esa $E_p$ se transforma en $49\text{ J}$ de Energía Cinética ($E_c$)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>¿Qué fuerza neta se necesita aplicar a una masa de $2\text{ kg}$ para que acelere a $3\text{ m/s}^2$?</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $F = m \cdot a = 2\text{ kg} \cdot 3\text{ m/s}^2 = 6\text{ N}$.
            </div>
        </div>

        <!-- 5. Hidrostática e Hidrodinámica -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Hidrostática e Hidrodinámica</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia el comportamiento de los fluidos en reposo y en movimiento[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Presión Hidrostática Absoluta:</strong> $P = P_0 + \rho \cdot g \cdot h$ (donde $P_0$ es la presión atmosférica en la superficie)[cite: 1].</p>
            <p>• <strong>Principio de Pascal:</strong> La presión aplicada a un fluido encerrado se transmite con igual intensidad en todas direcciones[cite: 1].</p>
            <p>• <strong>Principio de Arquímedes:</strong> Todo cuerpo sumergido experimenta un empuje vertical hacia arriba igual al peso del fluido desalojado ($E = \rho_{fluido} \cdot g \cdot V_{desalojado}$)[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Aclaraciones de Hidrodinámica:</strong>
                <br>• <strong>Continuidad:</strong> En un flujo estacionario e incompresible, sin acumulación, el caudal se conserva ($Q = A_1 v_1 = A_2 v_2$)[cite: 1].
                <br>• <strong>Bernoulli:</strong> La relación $P + \frac{1}{2}\rho v^2 + \rho g h = \text{cte}$ se aplica bajo condiciones ideales de flujo estacionario e incompresible a lo largo de una línea de corriente[cite: 1].
                <br>• <strong>Ejemplo en tuberías:</strong> Cuando un fluido circula por una tubería que se estrecha, su velocidad aumenta y, bajo determinadas condiciones, su presión disminuye[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Presión Absoluta:</strong> $P = P_0 + \rho \cdot g \cdot h$[cite: 1].</li>
                    <li><strong>Empuje:</strong> $E = \rho_{fluido} \cdot g \cdot V_{desalojado}$[cite: 1].</li>
                    <li><strong>Continuidad / Bernoulli:</strong> $A_1 v_1 = A_2 v_2 \quad | \quad P + \frac{1}{2}\rho v^2 + \rho g h = \text{constante}$[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Un buzo se encuentra sumergido a $10\text{ m}$ de profundidad en el mar ($\rho = 1025\text{ kg/m}^3$, $g = 9.8\text{ m/s}^2$). Si la presión en la superficie es $P_0 = 101325\text{ Pa}$, hallar la presión absoluta que soporta[cite: 1].</p>
                <p>• <strong>Paso 1 (Datos):</strong> $P_0 = 101325\text{ Pa}$, $\rho = 1025\text{ kg/m}^3$, $g = 9.8\text{ m/s}^2$, $h = 10\text{ m}$[cite: 1].</p>
                <p>• <strong>Paso 2 (Presión manométrica):</strong> $P_{man} = \rho \cdot g \cdot h = 1025 \cdot 9.8 \cdot 10 = 100450\text{ Pa}$[cite: 1].</p>
                <p>• <strong>Paso 3 (Presión absoluta):</strong> $P = P_0 + P_{man} = 101325 + 100450 = 201775\text{ Pa}$[cite: 1].</p>
                <p>• <strong>Paso 4 (Resultado):</strong> $P \approx 201.78\text{ kPa}$ (aproximadamente $2\text{ atm}$)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Un objeto de volumen $V = 0.02\text{ m}^3$ se sumerge completamente en agua ($\rho = 1000\text{ kg/m}^3$). Calculá el empuje que experimenta.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $E = \rho \cdot g \cdot V = 1000\text{ kg/m}^3 \cdot 9.8\text{ m/s}^2 \cdot 0.02\text{ m}^3 = 196\text{ N}$.
            </div>
        </div>

        <!-- 6. Viscosidad y Fenómenos de Transporte -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Viscosidad, Ley de Poiseuille y Transporte</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Describe el flujo de fluidos reales considerando la fricción interna y los mecanismos moleculares de transporte[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Ley de Poiseuille:</strong> Se aplica al flujo laminar de un fluido newtoniano por un tubo cilíndrico: $Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$. El caudal depende fuertemente del radio ($Q \propto r^4$)[cite: 1].</p>
            <p>• <strong>Ley de Fick:</strong> El flujo de difusión es proporcional al gradiente de concentración ($J = -D \cdot \frac{\Delta C}{\Delta x}$)[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Correcciones de transporte:</strong>
                <br>• <strong>Ósmosis:</strong> Existe un movimiento neto de agua a través de una membrana semipermeable hacia el lado con mayor concentración efectiva de solutos, bajo determinadas condiciones[cite: 1].
                <br>• <strong>Fenómenos de transporte:</strong> Los fenómenos de transporte se relacionan mediante gradientes, flujos, difusión, convección, viscosidad y sedimentación (la viscosidad es una propiedad del fluido, no una etapa posterior a la difusión)[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Poiseuille:</strong> Caudal en tubos proporcional al radio a la cuarta potencia ($r^4$)[cite: 1].</li>
                    <li><strong>Difusión (Fick):</strong> Transporte pasivo a favor de gradiente de concentración[cite: 1].</li>
                    <li><strong>Ósmosis:</strong> Movimiento neto de solvente a través de membrana semipermeable[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo conceptual</strong>
                <p><strong>Enunciado:</strong> ¿Cómo impacta reducir a la mitad el radio de un conducto según Poiseuille?[cite: 1]</p>
                <p>• <strong>Paso 1:</strong> La relación del caudal con el radio es de cuarta potencia ($r^4$)[cite: 1].</p>
                <p>• <strong>Paso 2:</strong> Si el radio pasa a ser $r/2$, el factor en el caudal es $(1/2)^4 = 1/16$[cite: 1].</p>
                <p>• <strong>Paso 3 (Conclusión):</strong> El caudal se reduce a la dieciseisava parte de su valor original[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar qué mecanismo de transporte es más rápido a distancias grandes: ¿la difusión pura o la convección de un fluido completo?</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> La convección, ya que desplaza la masa completa del fluido impulsada por trabajo mecánico (ej: bombeo).
            </div>
        </div>
    </div>
    /* Estilos específicos para Biología */
        .module-biologia .subject-header { background-color: var(--bg-biologia); color: var(--color-biologia); border: 1px solid var(--border-biologia); }
        .module-biologia .topic-card { border-color: var(--border-biologia); }
        .module-biologia .example-box { border-left-color: var(--color-biologia); background-color: var(--bg-biologia); }
        .module-biologia .synoptic-box { border-color: var(--color-biologia); }
        .module-biologia .synoptic-box li::before { color: var(--color-biologia); }
/* Estilos específicos para Biología */
        .module-biologia .subject-header { background-color: var(--bg-biologia); color: var(--color-biologia); border: 1px solid var(--border-biologia); }
        .module-biologia .topic-card { border-color: var(--border-biologia); }
        .module-biologia .example-box { border-left-color: var(--color-biologia); background-color: var(--bg-biologia); }
        .module-biologia .synoptic-box { border-color: var(--color-biologia); }
        .module-biologia .synoptic-box li::before { color: var(--color-biologia); }
        <!-- ==================== BLOQUE 3: BIOLOGÍA ==================== -->
    <div class="module-biologia">
        <h2 class="subject-header">🧬 Biología</h2>

        <!-- 1. La Célula y Organelos -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>La Célula: Estructura y Organelos</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Describe la unidad fundamental de los seres vivos y las funciones biológicas de sus componentes subcelulares[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Procariota:</strong> Célula sin núcleo delimitado por membrana (ej: bacterias)[cite: 1].</p>
            <p>• <strong>Eucariota:</strong> Célula con núcleo organizado y organelos membranosos especializados[cite: 1].</p>
            <p>• <strong>Núcleo:</strong> Contiene y resguarda el material genético[cite: 1].</p>
            <p>• <strong>Mitocondria:</strong> Organela encargada de la producción de energía (ATP)[cite: 1].</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Estructura celular:</strong> Membrana plasmática, Citoplasma, Material genético[cite: 1].</li>
                    <li><strong>Sistemas membranosos:</strong> Retículo Endoplasmático (síntesis) $\to$ Aparato de Golgi (empaquetado y envío)[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Identificar qué organela se desarrollará en mayor proporción en células con alta demanda energética (como las células musculares)[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar concepto):</strong> La demanda energética requiere síntesis masiva de ATP[cite: 1].</p>
                <p>• <strong>Paso 2 (Reconocer elementos):</strong> La organela especializada en la respiración aeróbica y obtención de ATP es la mitocondria[cite: 1].</p>
                <p>• <strong>Paso 3 (Relacionar):</strong> Estructuras con mayor trabajo mecánico consumen más ATP $\to$ requieren mayor densidad mitocondrial[cite: 1].</p>
                <p>• <strong>Paso 4 (Explicar conclusión):</strong> Las células musculares poseen abundante cantidad de mitocondrias en su citoplasma[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar qué organela celular es la responsable directa del ensamblado de proteínas a partir de la información genética.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Los ribosomas.
            </div>
        </div>

        <!-- 2. Metabolismo Energético -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Metabolismo Energético: Respiración Celular y Fotosíntesis</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia los procesos bioquímicos mediante los cuales las células transforman y obtienen energía química útil[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Respiración Celular Aeróbica:</strong> Ocurre en tres fases principales: Glucólisis (citoplasma), Ciclo de Krebs (matriz mitocondrial) y Cadena respiratoria / Fosforilación oxidativa (membrana interna mitocondrial)[cite: 1].</p>
            <p>• <strong>Fotosíntesis:</strong> Transforma energía lumínica en energía química sintetizando nutrientes en los cloroplastos[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificación conceptual precisa:</strong> La respiración celular oxida nutrientes, como la glucosa, y produce ATP (en lugar de la metáfora simplificada de "quemar glucosa")[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Respiración Celular:</strong> Oxidación de glucosa $\to$ Glucólisis $\to$ Krebs $\to$ Cadena respiratoria $\to$ Producción de ATP[cite: 1].</li>
                    <li><strong>Fotosíntesis:</strong> Etapa fotoquímica (captación de luz en tilacoides) $\to$ Ciclo de Calvin (fijación de $CO_2$ en estroma)[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Explicar el rol del oxígeno gaseoso ($O_2$) en la respiración celular aeróbica[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar la fase):</strong> Ocurre en la membrana interna de la mitocondria durante la Cadena Respiratoria[cite: 1].</p>
                <p>• <strong>Paso 2 (Reconocer su función):</strong> El $O_2$ actúa como el aceptor final de electrones e hidrógenos[cite: 1].</p>
                <p>• <strong>Paso 3 (Relacionar producto):</strong> Al aceptar electrones y protones, el oxígeno se reduce formando agua ($H_2O$)[cite: 1].</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> Sin oxígeno, la cadena de transporte se bloquea y la producción eficiente de ATP se detiene[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>¿En qué región concreta de la célula eucariota se lleva a cabo la Glucólisis?</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> En el citoplasma (o citosol).
            </div>
        </div>

        <!-- 3. Ciclo Celular: Mitosis y Meiosis -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Ciclo Celular: Mitosis y Meiosis</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Comprende los mecanismos de división nuclear y celular para la reproducción de tejidos o la formación de gametos[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Fases ordenadas de la división:</strong> Profase, Metafase, Anafase, Telofase[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificaciones conceptuales precisas:</strong>
                <br>• <strong>Mitosis:</strong> Forma dos células hijas con el mismo número de cromosomas y, en general, la misma información genética[cite: 1].
                <br>• <strong>Meiosis:</strong> Genera gametos genéticamente diversos mediante recombinación (crossing-over) y distribución independiente de cromosomas[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Mitosis:</strong> Célula $2n \to 2$ células $2n$ (Crecimiento y renovación tisular)[cite: 1].</li>
                    <li><strong>Meiosis:</strong> Célula $2n \to 4$ gametos $n$ (Reducción cromosómica y diversidad genética)[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Comparar la dotación cromosómica de una célula de la piel y un espermatozoide en una especie con $2n = 46$[cite: 1].</p>
                <p>• <strong>Paso 1 (Identificar proceso de origen):</strong> Célula de piel $\to$ Mitosis; Espermatozoide $\to$ Meiosis[cite: 1].</p>
                <p>• <strong>Paso 2 (Evaluar ploidía):</strong> La célula somática mantiene la dotación diploide ($2n$); la germinal es haploide ($n$)[cite: 1].</p>
                <p>• <strong>Paso 3 (Calcular valores):</strong> Piel $= 46$ cromosomas; Espermatozoide $= 46 / 2 = 23$ cromosomas[cite: 1].</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> La mitosis conserva la cantidad de cromosomas ($46$), mientras la meiosis la reduce a la mitad ($23$)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar en qué fase específica de la división celular los cromosomas se alinean en el plano ecuatorial de la célula.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> En la Metafase.
            </div>
        </div>

        <!-- 4. Genética y Herencia Mendelia -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Genética, Genoma y Herencia Mendelia</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia los mecanismos de transmisión de la información hereditaria y la expresión del genotipo en el fenotipo[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Alelo:</strong> Variante posible de un gen en un locus determinado[cite: 1].</p>
            <p>• <strong>Genotipo / Fenotipo:</strong> Genotipo es la combinación alélica; fenotipo es la característica observable[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificaciones conceptuales precisas:</strong>
                <br>• <strong>Genoma:</strong> Conjunto completo del material genético de un organismo[cite: 1].
                <br>• <strong>Gen:</strong> Segmento de ADN que contiene información para producir un producto funcional, como un ARN o una proteína, según el caso[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Genotipo:</strong> Homocigota ($AA$ / $aa$) | Heterocigota ($Aa$)[cite: 1].</li>
                    <li><strong>Cuadro de Punnett:</strong> Matriz probabilística para predecir proporciones genotípicas y fenotípicas[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Predecir las proporciones del cruce monohíbrido entre dos individuos heterocigotas ($Aa \times Aa$), donde el alelo $A$ es dominante (color rojo) y $a$ es recesivo (color blanco)[cite: 1].</p>
                <p>• <strong>Paso 1 (Gametos):</strong> Cada padre produce gametos $A$ ($50\%$) y $a$ ($50\%$)[cite: 1].</p>
                <p>• <strong>Paso 2 (Cruzamiento):</strong> Combinaciones posibles en el Cuadro de Punnett: $AA$, $Aa$, $Aa$, $aa$[cite: 1].</p>
                <p>• <strong>Paso 3 (Proporción Genotípica):</strong> $25\%\text{ } AA$, $50\%\text{ } Aa$, $25\%\text{ } aa$ (Relación 1:2:1)[cite: 1].</p>
                <p>• <strong>Paso 4 (Proporción Fenotípica):</strong> $75\%$ de individuos con fenotipo dominante (rojo) y $25\%$ con fenotipo recesivo (blanco)[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Al cruzar un individuo homocigota recesivo ($aa$) con un heterocigota ($Aa$), ¿qué porcentaje de la descendencia se espera que exprese el fenotipo recesivo?</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $50\%$ (combinaciones resultantes: $Aa$, $Aa$, $aa$, $aa$).
            </div>
        </div>

        <!-- 5. Expresión Génica, Evolución y Taxonomía -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Expresión Génica, Evolución y Clasificación Taxonómica</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Comprende el flujo de la información genética, los mecanismos de cambio evolutivo en poblaciones y la ordenación de la diversidad biológica[cite: 1].</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Dogma Molecular:</strong> Replicación ($\text{ADN} \to \text{ADN}$) $\to$ Transcripción ($\text{ADN} \to \text{ARN}$) $\to$ Traducción ($\text{ARN} \to \text{Proteína}$)[cite: 1].</p>

            <div class="warning-box">
                <strong>⚠️ Modificaciones conceptuales precisas:</strong>
                <br>• <strong>Traducción:</strong> Los codones especifican aminoácidos o señales de inicio y terminación durante la traducción[cite: 1].
                <br>• <strong>Evolución:</strong> La selección natural puede aumentar la frecuencia de variantes ventajosas en un determinado ambiente (evitando la simplificación de "favorece al más fuerte")[cite: 1].
                <br>• <strong>Taxonomía:</strong> Los organismos se clasifican en grandes grupos taxonómicos, como dominios y reinos, según características compartidas y relaciones evolutivas[cite: 1].
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Flujo genético:</strong> ADN $\to$ ARNm (núcleo) $\to$ Proteína en ribosoma (código genético leído por codones)[cite: 1].</li>
                    <li><strong>Evolución:</strong> Mutación (fuente de variabilidad) + Selección natural (frecuencia alélica diferencial)[cite: 1].</li>
                    <li><strong>Taxonomía:</strong> Nomenclatura binomial (<em>Género especie</em>) y clasificación en dominios y reinos[cite: 1].</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo conceptual paso a paso</strong>
                <p><strong>Enunciado:</strong> Explicar cómo un cambio puntual en el ADN (mutación) puede alterar una proteína[cite: 1].</p>
                <p>• <strong>Paso 1:</strong> La mutación modifica una base nitrogenada en la secuencia del gen en el ADN[cite: 1].</p>
                <p>• <strong>Paso 2:</strong> Durante la transcripción, la secuencia del ARNm copia ese cambio[cite: 1].</p>
                <p>• <strong>Paso 3:</strong> Durante la traducción, el codón alterado puede especificar un aminoácido diferente[cite: 1].</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> Al cambiar la secuencia de aminoácidos, la estructura y función de la proteína resultante pueden modificarse[cite: 1].</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar cuál es la estructura formada por un triplete de bases nitrogenadas en el ARNm que especifica un aminoácido.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Un codón.
            </div>
        </div>
    </div>
    /* Estilos específicos para Matemática */
        .module-matematica .subject-header { background-color: var(--bg-matematica); color: var(--color-matematica); border: 1px solid var(--border-matematica); }
        .module-matematica .topic-card { border-color: var(--border-matematica); }
        .module-matematica .example-box { border-left-color: var(--color-matematica); background-color: var(--bg-matematica); }
        .module-matematica .synoptic-box { border-color: var(--color-matematica); }
        .module-matematica .synoptic-box li::before { color: var(--color-matematica); }
        <!-- ==================== BLOQUE 4: MATEMÁTICA ==================== -->
    <div class="module-matematica">
        <h2 class="subject-header">📐 Matemática</h2>

        <!-- 1. Base Numérica, Notación Científica y Proporciones -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Base Numérica, Notación Científica y Proporciones</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Comprende las operaciones numéricas fundamentales, el manejo de escalas con notación científica y las relaciones de proporcionalidad.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Notación Científica:</strong> Expresa números mediante $a \times 10^n$ (donde $1 \le |a| < 10$).</p>
            <p>• <strong>Porcentaje:</strong> Razón que representa una fracción de 100 partes iguales.</p>

            <div class="warning-box">
                <strong>⚠️ Aclaración sobre Regla de Tres:</strong> La aplicación de la regla de tres simple supone que existe una relación de proporcionalidad estricta entre las magnitudes involucradas.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Operaciones base:</strong> Fracciones, potencias y raíces (operaciones inversas).</li>
                    <li><strong>Notación científica:</strong> $a \times 10^n$ (exponente negativo para números $< 1$; positivo para números $> 10$).</li>
                    <li><strong>Proporcionalidad:</strong> Directa (ambas crecen) | Inversa (una crece, la otra decrece).</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Si $5\text{ análisis}$ cuestan $\$500$, suponiendo proporcionalidad estricta entre precio y cantidad, calcular el costo de $8\text{ análisis}$.</p>
                <p>• <strong>Paso 1 (Identificar datos):</strong> $5\text{ unidades} \to \$500$; buscamos el precio $x$ para $8\text{ unidades}$.</p>
                <p>• <strong>Paso 2 (Elegir procedimiento):</strong> Regla de tres directa: $x = \frac{8 \cdot 500}{5}$.</p>
                <p>• <strong>Paso 3 (Resolver):</strong> $x = \frac{4000}{5} = \$800$.</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> Los $8\text{ análisis}$ cuestan $\$800$.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Expresá el número $0.000000045$ en notación científica.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $4.5 \times 10^{-8}$ (se desplaza la coma 8 lugares a la derecha).
            </div>
        </div>

        <!-- 2. Ecuaciones, Despejes y Sistemas -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Ecuaciones, Despejes y Sistemas de Ecuaciones</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Aísla incógnitas en planteos algebraicos aplicando operaciones inversas a ambos lados de la igualdad.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Ecuación Lineal:</strong> Igualdad de primer grado resoluble por despeje directo.</p>
            <p>• <strong>Ecuación Cuadrática:</strong> De la forma $ax^2 + bx + c = 0$, resoluble con la fórmula resolvente $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.</p>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Despeje:</strong> Aplicar operaciones inversas manteniendo el equilibrio de la igualdad.</li>
                    <li><strong>Sistemas:</strong> Dos o más incógnitas que deben satisfacer simultáneamente varias ecuaciones.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Despejar la incógnita $x$ en la ecuación $2x + 3 = 11$.</p>
                <p>• <strong>Paso 1 (Identificar estructura):</strong> La incógnita $x$ está multiplicada por $2$ y sumada a $3$.</p>
                <p>• <strong>Paso 2 (Restar constante):</strong> Restamos $3$ a ambos lados: $2x = 11 - 3 \implies 2x = 8$.</p>
                <p>• <strong>Paso 3 (Dividir coeficiente):</strong> Dividimos por $2$ a ambos lados: $x = \frac{8}{2} = 4$.</p>
                <p>• <strong>Paso 4 (Verificación):</strong> Reemplazamos $x = 4 \implies 2(4) + 3 = 8 + 3 = 11$. La igualdad se cumple.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Resolvé la ecuación cuadrática $x^2 - 5x + 6 = 0$ identificando $a, b, c$ y aplicando la fórmula resolvente.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $a=1, b=-5, c=6 \implies x = \frac{5 \pm \sqrt{25 - 24}}{2} = \frac{5 \pm 1}{2}$. Las soluciones son $x_1 = 3$ y $x_2 = 2$.
            </div>
        </div>

        <!-- 3. Funciones, Logaritmos, Probabilidad y Estadística -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Funciones, Logaritmos, Probabilidad y Estadística</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia los modelos de relación entre variables, la cuantificación de eventos aleatorios y la inferencia a partir de datos.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Funciones Exponenciales y Logarítmicas:</strong> Las funciones exponenciales pueden modelar crecimientos o decrecimientos rápidos; el logaritmo es su función inversa y permite trabajar con escalas multiplicativas.</p>
            <p>• <strong>Probabilidad:</strong> Un evento es un resultado o conjunto de resultados posibles dentro de un espacio muestral.</p>

            <div class="warning-box">
                <strong>⚠️ Definición de Prueba de Hipótesis:</strong> Una prueba de hipótesis evalúa si una diferencia observada es compatible con el azar bajo un determinado modelo estadístico.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Funciones:</strong> Lineal ($y=mx+b$) | Cuadrática ($y=ax^2+bx+c$) | Exponencial y Logarítmica.</li>
                    <li><strong>Probabilidad:</strong> $P(\text{Evento}) = \frac{\text{Casos favorables}}{\text{Casos posibles}}$ (en eventos equiprobables).</li>
                    <li><strong>Estadística:</strong> Descriptiva (resume datos con media/desvío) | Inferencia (prueba de hipótesis).</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Calcular la probabilidad simple de obtener un número par al lanzar un dado justo de 6 caras.</p>
                <p>• <strong>Paso 1 (Casos posibles):</strong> El espacio muestral es $\{1, 2, 3, 4, 5, 6\}$, por lo que hay 6 casos posibles.</p>
                <p>• <strong>Paso 2 (Casos favorables):</strong> Los números pares son $\{2, 4, 6\}$, por lo que hay 3 casos favorables.</p>
                <p>• <strong>Paso 3 (Aplicar fórmula):</strong> $P(\text{Par}) = \frac{3}{6} = \frac{1}{2} = 0.5$.</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> La probabilidad es del $50\%$.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Sabiendo que $10^2 = 100$, indicá el valor del logaritmo en base 10: $\log_{10}(100)$.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $\log_{10}(100) = 2$, ya que el logaritmo es la función inversa de la potencia.
            </div>
        </div>

        <!-- 4. Cálculo: Derivada e Integral -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Cálculo: Derivada e Integral</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia las tasas de cambio instantáneas y la acumulación continua de cantidades descritas por funciones.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Derivada ($f'(x)$):</strong> Representa geométricamente la <em>pendiente de la recta tangente</em> a la curva en un punto o la <em>tasa de cambio instantánea</em> de la función.</p>
            <p>• <strong>Integral Definida ($\int_{a}^{b} f(x)dx$):</strong> Representa geométricamente el <em>área acumulada bajo la curva</em> entre los límites $a$ y $b$.</p>

            <div class="warning-box">
                <strong>⚠️ Clarificación sobre Puntos Críticos:</strong> Si $f'(x) = 0$, se obtiene un punto crítico. Este puede corresponder a un máximo local, un mínimo local o a ninguno (como en un punto de silla con tangente horizontal); se necesitan otros criterios (como el signo de la derivada segunda) para determinarlo. Esto debe separarse del análisis de concavidad e inflexión.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Derivada:</strong> Pendiente de la recta tangente / Tasa de cambio instantánea $\to f'(x) = 0$ da puntos críticos.</li>
                    <li><strong>Integral:</strong> Operación inversa a la derivada $\to \int_{a}^{b} f(x)dx$ calcula el área bajo la curva.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Dada la función de posición $x(t) = t^2$ en metros, hallar la velocidad instantánea en $t = 3\text{ s}$ sabiendo que la derivada de $t^2$ es $2t$.</p>
                <p>• <strong>Paso 1 (Identificar concepto):</strong> La velocidad instantánea es la derivada de la posición: $v(t) = x'(t)$.</p>
                <p>• <strong>Paso 2 (Obtener la función derivada):</strong> $v(t) = 2t$.</p>
                <p>• <strong>Paso 3 (Evaluar en el punto):</strong> $v(3) = 2(3) = 6\text{ m/s}$.</p>
                <p>• <strong>Paso 4 (Conclusión):</strong> La pendiente de la recta tangente en $t = 3\text{ s}$ es $6$, lo que significa que la velocidad es de $6\text{ m/s}$.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Dada $f(x) = x^3$, cuya derivada es $f'(x) = 3x^2$, hallá la pendiente de la recta tangente en $x = 2$.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> $f'(2) = 3(2^2) = 3(4) = 12$.
            </div>
        </div>

        <!-- 5. Álgebra Lineal, Grafos y Optimización -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Álgebra Lineal, Teoría de Grafos y Optimización</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Procesa estructuras multidimensionales, representa redes de elementos interconectados y busca los valores óptimos de un sistema.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Vectores y Matrices:</strong> Listas y tablas organizadas de números para representar datos en múltiples dimensiones.</p>
            <p>• <strong>PCA (Análisis de Componentes Principales):</strong> Técnica de álgebra lineal para reducir la dimensión de un conjunto de datos sin perder información relevante.</p>
            <p>• <strong>Teoría de Grafos:</strong> Estructuras formadas por <strong>Nodos</strong> (elementos) y <strong>Aristas</strong> (conexiones) para representar redes de interacción.</p>

            <div class="warning-box">
                <strong>⚠️ Concepto de Optimización:</strong> La optimización puede utilizarse para encontrar máximos o mínimos de una función y también para ajustar modelos matemáticos a datos experimentales.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Álgebra Lineal:</strong> Operaciones con matrices $\to$ Reducción de dimensiones (PCA).</li>
                    <li><strong>Grafos:</strong> Nodos (puntos) + Aristas (líneas) $\to$ Representación de redes complejas.</li>
                    <li><strong>Optimización:</strong> Búsqueda de máximos/mínimos o ajuste de parámetros a datos reales.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo conceptual paso a paso</strong>
                <p><strong>Enunciado:</strong> Representar una red donde 3 personas (A, B, C) están conectadas si son amigas: A es amiga de B, y B es amiga de C.</p>
                <p>• <strong>Paso 1 (Identificar Nodos):</strong> Los elementos son las 3 personas $\to$ Nodos = $\{A, B, C\}$.</p>
                <p>• <strong>Paso 2 (Identificar Aristas):</strong> Las conexiones son las relaciones $\to$ Aristas = $\{(A,B), (B,C)\}$.</p>
                <p>• <strong>Paso 3 (Conclusión):</strong> Se forma un grafo de 3 nodos y 2 aristas.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Si agregamos una amistad directa entre A y C en el ejemplo anterior, ¿cuántas aristas tendrá el grafo final?</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Tendrá 3 aristas: $\{(A,B), (B,C), (A,C)\}$.
            </div>
        </div>
    </div>
    /* Estilos específicos para Programación */
        .module-programacion .subject-header { background-color: var(--bg-programacion); color: var(--color-programacion); border: 1px solid var(--border-programacion); }
        .module-programacion .topic-card { border-color: var(--border-programacion); }
        .module-programacion .example-box { border-left-color: var(--color-programacion); background-color: var(--bg-programacion); }
        .module-programacion .synoptic-box { border-color: var(--color-programacion); }
        .module-programacion .synoptic-box li::before { color: var(--color-programacion); }
        .code-container { background-color: #0f172a; color: #f8fafc; padding: 16px 20px; border-radius: 12px; font-family: 'JetBrains Mono', monospace; font-size: 0.88rem; overflow-x: auto; margin: 12px 0; }
        <!-- ==================== BLOQUE 5: PROGRAMACIÓN ==================== -->
    <div class="module-programacion">
        <h2 class="subject-header">💻 Programación (Python)</h2>

        <!-- 1. Algoritmos, Variables y Estructuras de Control -->
        <div class="topic-card">
            <span class="badge badge-reconocer">🟢 RECONOCER</span>
            <h3>Algoritmos, Variables y Estructuras de Control</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Estudia el diseño de secuencias lógicas e inequívocas de pasos (algoritmos) para procesar datos y tomar decisiones en un lenguaje de programación.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Tipos de datos básicos:</strong> Enteros (`int`), Decimales (`float`), Texto (`str`) y Booleanos (`bool`).</p>
            <p>• <strong>Condicionales (`if` / `else`):</strong> Permiten bifurcar el flujo de ejecución según el cumplimiento de una condición lógica.</p>

            <div class="warning-box">
                <strong>⚠️ Definición del Bucle `while`:</strong> El bucle `while` repite la ejecución de un bloque de código mientras una condición dada sea verdadera (a diferencia de `for`, que suele iterar sobre una colección o rango predefinido).
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Estructura general:</strong> Datos de entrada $\to$ Algoritmo $\to$ Resultado de salida.</li>
                    <li><strong>Bucles:</strong> `for` (iteración sobre colecciones) | `while` (repetición condicionada).</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso</strong>
                <p><strong>Enunciado:</strong> Escribir un script que evalúe si un valor de pH es ácido ($< 7.0$) o básico/neutro.</p>
                <div class="code-container">
ph = 6.5

# Paso 1: Evaluar la condición lógica
if ph < 7.0:
    # Paso 2: Ejecutar bloque si es verdadero
    print("La solución es ácida")
else:
    # Paso 3: Ejecutar bloque alternativo
    print("La solución es neutra o básica")
                </div>
                <p>• <strong>Resultado:</strong> Imprime `"La solución es ácida"` porque $6.5 < 7.0$.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Escribí una estructura `if` / `else` que verifique si una variable `temperatura` es mayor a $37.5$ y muestre `"Fiebre"` o `"Normal"`.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong>
                <div class="code-container">
if temperatura > 37.5:
    print("Fiebre")
else:
    print("Normal")
                </div>
            </div>
        </div>

        <!-- 2. Colecciones, Búsqueda y Archivos -->
        <div class="topic-card">
            <span class="badge badge-resolver">🔴 RESOLVER</span>
            <h3>Colecciones, Búsqueda, Ordenamiento y Archivos</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Almacena conjuntos de datos estructurados en memoria y gestiona la lectura y escritura de archivos de datos externos.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Listas:</strong> Colecciones ordenadas de elementos modificables accesibles por índice numérico (`lista[0]`).</p>
            <p>• <strong>Archivos CSV:</strong> Archivos de texto estructurados en filas y columnas; suelen utilizar comas como separador, aunque pueden emplear otros delimitadores como tabuladores o puntos y comas.</p>

            <div class="warning-box">
                <strong>⚠️ Modificaciones técnicas precisas:</strong>
                <br>• <strong>Diccionarios:</strong> En Python moderno, los diccionarios conservan el orden de inserción, pero se accede a sus elementos mediante claves, no mediante índices.
                <br>• <strong>Búsqueda y Ordenamiento:</strong> Una colección ordenada permite utilizar algoritmos de búsqueda eficientes, como la búsqueda binaria, cuando corresponde.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Colecciones:</strong> Listas (acceso por índice) | Diccionarios (acceso por clave).</li>
                    <li><strong>Lectura de archivos:</strong> Sentencia `with open(...)` para garantizar el cierre seguro del archivo.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo resuelto paso a paso (Recorrer cadena y contar frecuencias)</strong>
                <p><strong>Enunciado:</strong> Contar la frecuencia de cada carácter en una cadena de texto almacenando los resultados en un diccionario.</p>
                <div class="code-container">
texto = "GATTACA"
frecuencias = {}

# Paso 1: Recorrer cada carácter de la cadena
for caracter in texto:
    # Paso 2: Actualizar el contador en el diccionario usando la clave
    frecuencias[caracter] = frecuencias.get(caracter, 0) + 1

# Paso 3: Mostrar el resultado
print(frecuencias)
                </div>
                <p>• <strong>Resultado:</strong> `{'G': 1, 'A': 3, 'T': 2, 'C': 1}`.</p>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Escribí el patrón de código seguro en Python para abrir y leer un archivo de texto llamado `"datos.txt"` utilizando `with open`.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong>
                <div class="code-container">
with open("datos.txt", "r") as archivo:
    contenido = archivo.read()
    print(contenido)
                </div>
            </div>
        </div>

        <!-- 3. Funciones, Excepciones y Control de Versiones -->
        <div class="topic-card">
            <span class="badge badge-entender">🟡 ENTENDER</span>
            <h3>Funciones, Manejo de Errores, Git y GitHub</h3>

            <div class="section-title">¿Qué es?</div>
            <p>Comprende la modularización del código en funciones reutilizables, la prevención de fallos en ejecución y el control de versiones colaborativo.</p>

            <div class="section-title">🔎 Ideas clave</div>
            <p>• <strong>Funciones (`def`):</strong> Bloques de código modularizados que reciben parámetros de entrada y devuelven valores mediante `return`.</p>
            <p>• <strong>Excepciones (`try` / `except`):</strong> Estructuras de control que previenen que el programa se detenga abruptamente ante errores inesperados.</p>

            <div class="warning-box">
                <strong>⚠️ Programación como herramienta universal:</strong> La programación es una herramienta de trabajo habitual en proyectos de automatización, análisis de datos, ingeniería y desarrollo de software.
            </div>

            <div class="synoptic-box">
                <strong>📌 Cuadro sinóptico</strong>
                <ul>
                    <li><strong>Modularización:</strong> Funciones `def` para evitar la repetición de código.</li>
                    <li><strong>Git y GitHub:</strong> Git registra el historial local de cambios; GitHub permite alojar y colaborar en repositorios remotos.</li>
                </ul>
            </div>

            <div class="example-box">
                <strong>🧮 Ejemplo conceptual paso a paso</strong>
                <p><strong>Enunciado:</strong> Definir una función que calcule el promedio de una lista de números.</p>
                <div class="code-container">
def calcular_promedio(numeros):
    # Paso 1: Sumar elementos y contar la cantidad
    suma_total = sum(numeros)
    cantidad = len(numeros)
    
    # Paso 2: Calcular el cociente
    return suma_total / cantidad

# Paso 3: Llamar a la función con datos de prueba
resultado = calcular_promedio([10, 20, 30])
print(resultado)  # Muestra 20.0
                </div>
            </div>

            <div class="practice-box">
                <strong>✏️ Practicá</strong>
                <p>Indicar qué herramienta se utiliza para guardar el historial local de cambios en un proyecto de código antes de subirlo a GitHub.</p>
            </div>

            <div class="solution-box">
                <strong>✅ Solución:</strong> Git.
            </div>
        </div>
    </div>

    <!-- ==================== FORMULARIO UNIFICADO Y CONSTANTES ==================== -->
    <div class="topic-card" style="margin-top: 50px; border-color: #cbd5e1;">
        <h2 style="font-size: 1.5rem; color: #1e293b; margin-bottom: 15px;">📑 Hoja de Constantes y Formulario Unificado</h2>
        
        <p style="font-size: 0.9rem; margin-bottom: 20px;">
            Compendio unificado de fórmulas, constantes universales y ecuaciones clave para consulta durante la resolución de ejercicios.
        </p>

        <div class="ptable-container">
            <table class="ptable" style="text-align: left;">
                <thead>
                    <tr>
                        <th style="width: 20%;">Materia</th>
                        <th style="width: 35%;">Concepto / Magnitud</th>
                        <th style="width: 45%;">Fórmula / Valor Universal</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Química</strong></td>
                        <td>Número de Avogadro ($N_A$)</td>
                        <td>$N_A = 6.022 \times 10^{23}\text{ partículas/mol}$</td>
                    </tr>
                    <tr>
                        <td><strong>Química</strong></td>
                        <td>Molaridad ($M$) / pH</td>
                        <td>$M = \frac{\text{moles de soluto}}{\text{litros de solución}} \quad \vert{} \quad pH = -\log[H^+]$</td>
                    </tr>
                    <tr>
                        <td><strong>Física</strong></td>
                        <td>Aceleración de la gravedad ($g$)</td>
                        <td>$g \approx 9.8\text{ m/s}^2$</td>
                    </tr>
                    <tr>
                        <td><strong>Física</strong></td>
                        <td>Presión Hidrostática Absoluta</td>
                        <td>$P = P_0 + \rho \cdot g \cdot h$</td>
                    </tr>
                    <tr>
                        <td><strong>Física</strong></td>
                        <td>Empuje de Arquímedes</td>
                        <td>$E = \rho_{fluido} \cdot g \cdot V_{desalojado}$</td>
                    </tr>
                    <tr>
                        <td><strong>Física</strong></td>
                        <td>Ley de Poiseuille (Caudal)</td>
                        <td>$Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L} \quad (Q \propto r^4)$</td>
                    </tr>
                    <tr>
                        <td><strong>Matemática</strong></td>
                        <td>Resolvente Cuadrática</td>
                        <td>$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$</td>
                    </tr>
                    <tr>
                        <td><strong>Matemática</strong></td>
                        <td>Derivada / Integral</td>
                        <td>$f'(x) = \text{Pendiente tangente / Tasa de cambio} \quad \vert{} \quad \int_{a}^{b} f(x)dx = \text{Área bajo la curva}$</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
    
</div>
</body>
</html>
