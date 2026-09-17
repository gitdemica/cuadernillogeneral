<!doctype html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Cuadernillo General — Ciencias, Matemática y Programación</title>
<meta name="description" content="Cuadernillo general de Química, Física, Biología, Matemática y Programación (Python), con conceptos, ejemplos paso a paso y práctica.">
<script>window.MathJax={tex:{inlineMath:[['$','$'],['\\(','\\)']],displayMath:[['$$','$$'],['\\[','\\]']]},svg:{fontCache:'global'}};</script>
<script async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js"></script>
<style>
:root{--bg:#f6f4f1;--paper:#fff;--ink:#252329;--muted:#6f6a73;--line:#e5e0e5;--shadow:0 10px 28px rgba(35,28,40,.07);--radius:18px;--accent:#7c4d8f;}
*{box-sizing:border-box} html{scroll-behavior:smooth} body{margin:0;background:var(--bg);color:var(--ink);font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,Arial,sans-serif;line-height:1.65} a{color:inherit} .wrap{max-width:1180px;margin:auto;padding:24px} 
.hero{background:linear-gradient(135deg,#fff,#f2edf5);border:1px solid var(--line);border-radius:28px;padding:34px 30px;margin-bottom:22px;box-shadow:var(--shadow)} .hero h1{margin:.1em 0 .2em;font-size:clamp(2rem,4vw,3.2rem)} .hero p{color:var(--muted);max-width:820px} .nav{position:sticky;top:10px;z-index:10;display:flex;gap:8px;flex-wrap:wrap;background:rgba(246,244,241,.92);backdrop-filter:blur(10px);padding:10px;border:1px solid var(--line);border-radius:16px;margin-bottom:24px} .nav a{text-decoration:none;padding:7px 11px;border-radius:10px;background:#fff;border:1px solid var(--line);font-size:.92rem}
.module{background:var(--paper);border:1px solid var(--line);border-radius:var(--radius);padding:28px;margin:26px 0;box-shadow:var(--shadow)} .module h2{font-size:2rem;margin-top:0;padding-bottom:12px;border-bottom:2px solid var(--line)} .module h3{margin-top:28px;font-size:1.35rem} .module-quimica h2{color:#8b4b72} .module-fisica h2{color:#2f6f86} .module-biologia h2{color:#3e7b5d} .module-matematica h2{color:#7058a4} .module-programacion h2{color:#3f667f} .module-formulario h2{color:#8b6a3e}
.module h3{scroll-margin-top:90px} .module p{margin:.65em 0} .module ul,.module ol{padding-left:1.5rem} .module blockquote{border-left:4px solid #c9c0ca;padding-left:14px;color:var(--muted)} .module code{background:#f1eef2;padding:.12em .35em;border-radius:5px} pre{background:#15151b;color:#f6f3f8;padding:16px 18px;border-radius:14px;overflow:auto;border:1px solid #2b2930} pre code{background:transparent;padding:0;color:inherit}
.pt-guide{background:#faf7fb;border:1px solid #e6dbe9;border-radius:14px;padding:15px 18px;margin:12px 0 18px} .periodic-wrap{overflow-x:auto;padding-bottom:8px} .group-labels,.periodic-table{display:grid;grid-template-columns:repeat(18,minmax(74px,1fr));gap:5px;min-width:1450px} .group-labels span{text-align:center;color:var(--muted);font-size:.72rem} .pt-row{display:contents} .pt-cell{min-height:86px;border:1px solid rgba(0,0,0,.08);border-radius:9px;padding:5px;display:flex;flex-direction:column;justify-content:space-between;box-shadow:0 2px 5px rgba(0,0,0,.03)} .pt-cell.empty{border-color:transparent;box-shadow:none} .pt-cell .z{font-size:.65rem;color:var(--muted)} .pt-cell strong{font-size:1.12rem;line-height:1.1} .pt-cell .name{font-size:.63rem;line-height:1.1;word-break:break-word} .alcalino{background:#ffe8dc} .alcalinoterreo{background:#fff1c9} .transicion{background:#e9e5ff} .metal{background:#e4f0f7} .metaloide{background:#e6f5df} .no-metal{background:#e8f7ed} .halogeno{background:#fff0f6} .gas-noble{background:#eee9ff} .lantanido{background:#f8e5f2} .actinido{background:#f2e3e9} .legend{display:flex;flex-wrap:wrap;gap:7px;margin-top:12px} .legend-item{padding:5px 9px;border:1px solid rgba(0,0,0,.08);border-radius:999px;font-size:.75rem}
.fblock{min-width:1450px;margin-top:12px} .f-label{font-weight:700;margin:10px 0 4px} .f-row{display:grid;grid-template-columns:repeat(15,minmax(74px,1fr));gap:5px;margin-left:160px}
footer{text-align:center;color:var(--muted);padding:28px} .print-note{font-size:.9rem;color:var(--muted)}
@media(max-width:700px){.wrap{padding:12px} .module{padding:20px 16px} .hero{padding:25px 20px} .nav{position:static}}
@media print{body{background:#fff} .nav{display:none} .hero,.module{box-shadow:none;border-color:#ccc} .module{break-inside:auto} a{text-decoration:none}}
</style>
</head>
<body>
<div class="wrap">
<header class="hero"><h1>📚 Cuadernillo General</h1><p>Material de estudio de <b>Química, Física, Biología, Matemática y Programación (Python)</b>. Cada tema combina conceptos, ideas clave, ejemplos resueltos y práctica. Está pensado como material general de consulta y preparación, sin atarlo a una carrera específica.</p><p class="print-note">🟢 Reconocer · 🟡 Entender · 🔴 Resolver</p></header>
<nav class="nav"><a href="#quimica">🧪 Química</a><a href="#fisica">⚡ Física</a><a href="#biologia">🧬 Biología</a><a href="#matematica">📐 Matemática</a><a href="#programacion">💻 Programación</a><a href="#formulario">📑 Formulario</a></nav>
<h1><a href="https://gitdemica.github.io/cuadernillogeneral/">cuadernillogeneral</a></h1>
<section id="quimica" class="module module-quimica"><h2>🧪 Química</h2>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Sistemas Materiales y Sustancias Puras</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia cómo se clasifica la materia según sus fases visibles y la forma en que sus componentes se dividen o descomponen.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Sistema Homogéneo:</strong> Presenta 1 sola fase continua con propiedades uniformes.</p>
<p>• <strong>Sistema Heterogéneo:</strong> Presenta 2 o más fases separadas por superficies de contacto (interfases).</p>
<p><strong>⚠️ Modificación conceptual precisa:</strong> Las mezclas pueden separarse mediante métodos físicos; en cambio, los compuestos pueden descomponerse en sustancias más simples mediante procesos químicos.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Mezclas:</strong> Composición variable $\to$ Separables por métodos físicos (filtración, destilación).</li>
<li><strong>Compuestos:</strong> Composición constante $\to$ Descomponibles por métodos químicos.</li>
<li><strong>Elementos:</strong> Sustancias fundamentales $\to$ No se descomponen químicamente.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Clasificar un recipiente que contiene agua líquida, cubos de hielo y arena en el fondo.</p>
<p>• <strong>Paso 1 (Identificar concepto):</strong> Determinar la cantidad de fases (porciones homogéneas físicamente diferenciables).</p>
<p>• <strong>Paso 2 (Reconocer elementos):</strong> Fase 1: agua líquida, Fase 2: hielo sólido, Fase 3: arena sólida.</p>
<p>• <strong>Paso 3 (Relacionar):</strong> Aunque el agua y el hielo son la misma sustancia ($H_2O$), están en estados distintos, formando 2 fases diferentes.</p>
<p>• <strong>Paso 4 (Explicar conclusión):</strong> Es un sistema heterogéneo formado por 3 fases y 2 componentes ($H_2O$ y arena).</p>
<p><strong>✏️ Practicá</strong></p>
<p>Un sistema contiene agua completamente saturada de sal con cristales de sal depositados en el fondo. Indicar número de fases y componentes.</p>
<p><strong>✅ Solución:</strong> Posee 2 fases (fase líquida salada + fase sólida de cristales de sal) y 2 componentes (agua y sal).</p>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Átomos, Estructura Atómica y Tabla Periódica</h3>
<p><strong>¿Qué es?</strong></p>
<p>Describe la organización interna del átomo y el ordenamiento de los elementos en la Tabla Periódica.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Número Atómico ($Z$):</strong> Cantidad de protones en el núcleo; define la identidad del elemento.</p>
<p>• <strong>Tabla Periódica:</strong> Ordena los elementos en grupos (columnas) y períodos (filas) según su número atómico.</p>
<p><strong>⚠️ Modificación conceptual precisa:</strong> El electrón posee carga negativa y se encuentra distribuido en la <em>nube electrónica / orbitales atómicos</em> (superando el concepto de órbita circular plana).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Núcleo:</strong> Protones (carga $+$) + Neutrones (sin carga).</li>
<li><strong>Electrón:</strong> Nube electrónica / orbitales (carga $-$).</li>
<li><strong>Grupos / Períodos:</strong> Elementos del mismo grupo poseen propiedades químicas relacionadas.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Determinar la cantidad de subpartículas de un átomo neutro de Sodio ($Na$) con $Z = 11$ y Número Másico $A = 23$.</p>
<p>• <strong>Paso 1:</strong> Identificar que $Z = \text{protones}$. Por lo tanto, tiene 11 protones.</p>
<p>• <strong>Paso 2:</strong> Al ser un átomo neutro, la cantidad de electrones iguala a los protones: 11 electrones.</p>
<p>• <strong>Paso 3:</strong> Calcular neutrones mediante $A - Z$: $23 - 11 = 12$ neutrones.</p>
<p>• <strong>Resultado:</strong> 11 protones, 11 electrones en la nube electrónica y 12 neutrones.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Un átomo neutro de Carbono posee $Z = 6$ y $A = 12$. Indicar cuántos electrones orbitan en su nube electrónica y cuántos neutrones posee en su núcleo.</p>
<p><strong>✅ Solución:</strong> Posee 6 electrones en su nube electrónica y 6 neutrones ($12 - 6 = 6$).</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Enlace Químico, Química Inorgánica y Sales</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia cómo los átomos se unen para alcanzar estabilidad y cómo se forman y nombran las sustancias inorgánicas.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Enlace Iónico:</strong> Metal + No metal (transferencia de electrones).</p>
<p>• <strong>Enlace Covalente:</strong> No metal + No metal (compartición de electrones).</p>
<p><strong>⚠️ Modificaciones conceptuales precisas:</strong>
• <strong>Química inorgánica:</strong> Estudia los compuestos que no se clasifican como orgánicos.
• <strong>Sales:</strong> Son compuestos iónicos; muchas de ellas se forman a partir de reacciones de neutralización ácido-base.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Iónico:</strong> Formación de cationes ($+$) y aniones ($-$).</li>
<li><strong>Covalente:</strong> Formación de moléculas por pares compartidos.</li>
<li><strong>Sales:</strong> Compuestos iónicos formados comúnmente por un catión metálico y un anión no metálico.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Explicar el tipo de enlace en el Fluoruro de Litio ($LiF$).</p>
<p>• <strong>Paso 1:</strong> Identificar los elementos: Litio ($Li$, metal alcalino) y Flúor ($F$, no metal halógeno).</p>
<p>• <strong>Paso 2:</strong> Analizar la interacción: el Litio cede 1 electrón formando $Li^+$; el Flúor acepta ese electrón formando $F^-$.</p>
<p>• <strong>Paso 3:</strong> Conclusión: Unión electrostática entre cationes y aniones $\to$ Enlace Iónico.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar qué tipo de enlace predomina en la molécula de agua ($H_2O$) sabiendo que el Hidrógeno y el Oxígeno son no metales.</p>
<p><strong>✅ Solución:</strong> Enlace Covalente, ya que ambos no metales comparten electrones.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Mol, Masa Molar y Conversiones</h3>
<p><strong>¿Qué es?</strong></p>
<p>Permite vincular la escala microscópica de átomos y moléculas con las masas medibles en laboratorio.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Mol:</strong> Cantidad de sustancia que contiene $6.022 \times 10^{23}$ partículas elementales (Número de Avogadro).</p>
<p>• <strong>Masa Molar ($M$):</strong> Masa en gramos de 1 mol de sustancia ($g/mol$).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Conversión:</strong> $\text{Moles } (n) = \frac{\text{Masa en gramos } (m)}{\text{Masa Molar } (M)}$.</li>
<li><strong>Partículas:</strong> $\text{Número de partículas} = n \times 6.022 \times 10^{23}$.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Calcular cuántos moles y cuántas moléculas hay en $36\text{ g}$ de agua ($H_2O$).</p>
<p>• <strong>Paso 1 (Identificar datos):</strong> $m = 36\text{ g}$. Masas atómicas: $H = 1\text{ g/mol}$, $O = 16\text{ g/mol}$.</p>
<p>• <strong>Paso 2 (Elegir fórmula):</strong> $M_{H_2O} = (2 \times 1) + 16 = 18\text{ g/mol}$. Luego $n = m / M$.</p>
<p>• <strong>Paso 3 (Reemplazar y aplicar):</strong> $n = 36\text{ g} / 18\text{ g/mol} = 2\text{ moles}$.</p>
<p>• <strong>Paso 4 (Resolver moléculas):</strong> $2\text{ moles} \times 6.022 \times 10^{23} = 1.2044 \times 10^{24}\text{ moléculas}$.</p>
<p>• <strong>Resultado:</strong> $2\text{ moles}$ que equivalen a $1.2044 \times 10^{24}\text{ moléculas}$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Calcular la cantidad de moles presentes en $88\text{ g}$ de dióxido de carbono ($CO_2$). (Masas atómicas: $C = 12\text{ g/mol}$, $O = 16\text{ g/mol}$).</p>
<p><strong>✅ Solución:</strong> $M_{CO_2} = 12 + (2 \times 16) = 44\text{ g/mol}$. Moles $= 88\text{ g} / 44\text{ g/mol} = 2\text{ moles}$.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Soluciones, Molaridad y pH</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia la cuantificación de concentraciones de solutos disueltos en líquidos y la medida de acidez.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Molaridad ($M$):</strong> $M = \frac{\text{moles de soluto}}{\text{litros de solución}}$.</p>
<p>• <strong>Escala de pH:</strong> $pH = -\log[H^+]$.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Molaridad:</strong> Unidades expresadas estrictamente en Moles por Litro ($mol/L$).</li>
<li><strong>pH:</strong> Medida logarítmica ( $pH &lt; 7$ Ácido | $pH = 7$ Neutro | $pH &gt; 7$ Básico ).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Se disuelven $0.5\text{ moles}$ de $HCl$ en agua hasta alcanzar $2\text{ litros}$ de solución. Hallar Molaridad y $pH$.</p>
<p>• <strong>Paso 1 (Datos):</strong> $n = 0.5\text{ mol}$, $V = 2\text{ L}$.</p>
<p>• <strong>Paso 2 (Aplicar Molaridad):</strong> $M = 0.5\text{ mol} / 2\text{ L} = 0.25\text{ M}$.</p>
<p>• <strong>Paso 3 (Aplicar pH):</strong> $[H^+] = 0.25\text{ M} \implies pH = -\log(0.25)$.</p>
<p>• <strong>Paso 4 (Resolver):</strong> $pH = 0.60$.</p>
<p>• <strong>Resultado:</strong> Solución $0.25\text{ M}$ con $pH = 0.60$ (altamente ácida).</p>
<p><strong>✏️ Practicá</strong></p>
<p>Se preparan $500\text{ mL}$ ($0.5\text{ L}$) de solución disolviendo $0.1\text{ moles}$ de un ácido fuerte. Calculá su Molaridad.</p>
<p><strong>✅ Solución:</strong> $M = 0.1\text{ mol} / 0.5\text{ L} = 0.2\text{ M}$.</p>
<h3>🧪 Tabla Periódica de los Elementos (Herramienta de Consulta)</h3>
<div class="pt-guide"><p><b>Z (número atómico):</b> cantidad de protones.</p><p><b>Período:</b> fila de la tabla.</p><p><b>Grupo:</b> columna; los elementos de una misma familia suelen compartir propiedades químicas relacionadas.</p><p><b>Importante:</b> es una herramienta de consulta; no es necesario memorizar los 118 elementos.</p></div>
<div class="periodic-wrap"><div class="group-labels"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span></div><div class="periodic-table"><div class="pt-row"><div class="pt-cell no-metal" title="Hidrógeno — Z=1, grupo 1, período 1"><span class="z">1</span><strong>H</strong><span class="name">Hidrógeno</span></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell gas-noble" title="Helio — Z=2, grupo 18, período 1"><span class="z">2</span><strong>He</strong><span class="name">Helio</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Litio — Z=3, grupo 1, período 2"><span class="z">3</span><strong>Li</strong><span class="name">Litio</span></div><div class="pt-cell alcalinoterreo" title="Berilio — Z=4, grupo 2, período 2"><span class="z">4</span><strong>Be</strong><span class="name">Berilio</span></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell metaloide" title="Boro — Z=5, grupo 13, período 2"><span class="z">5</span><strong>B</strong><span class="name">Boro</span></div><div class="pt-cell no-metal" title="Carbono — Z=6, grupo 14, período 2"><span class="z">6</span><strong>C</strong><span class="name">Carbono</span></div><div class="pt-cell no-metal" title="Nitrógeno — Z=7, grupo 15, período 2"><span class="z">7</span><strong>N</strong><span class="name">Nitrógeno</span></div><div class="pt-cell no-metal" title="Oxígeno — Z=8, grupo 16, período 2"><span class="z">8</span><strong>O</strong><span class="name">Oxígeno</span></div><div class="pt-cell halogeno" title="Flúor — Z=9, grupo 17, período 2"><span class="z">9</span><strong>F</strong><span class="name">Flúor</span></div><div class="pt-cell gas-noble" title="Neón — Z=10, grupo 18, período 2"><span class="z">10</span><strong>Ne</strong><span class="name">Neón</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Sodio — Z=11, grupo 1, período 3"><span class="z">11</span><strong>Na</strong><span class="name">Sodio</span></div><div class="pt-cell alcalinoterreo" title="Magnesio — Z=12, grupo 2, período 3"><span class="z">12</span><strong>Mg</strong><span class="name">Magnesio</span></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell empty"></div><div class="pt-cell metal" title="Aluminio — Z=13, grupo 13, período 3"><span class="z">13</span><strong>Al</strong><span class="name">Aluminio</span></div><div class="pt-cell metaloide" title="Silicio — Z=14, grupo 14, período 3"><span class="z">14</span><strong>Si</strong><span class="name">Silicio</span></div><div class="pt-cell no-metal" title="Fósforo — Z=15, grupo 15, período 3"><span class="z">15</span><strong>P</strong><span class="name">Fósforo</span></div><div class="pt-cell no-metal" title="Azufre — Z=16, grupo 16, período 3"><span class="z">16</span><strong>S</strong><span class="name">Azufre</span></div><div class="pt-cell halogeno" title="Cloro — Z=17, grupo 17, período 3"><span class="z">17</span><strong>Cl</strong><span class="name">Cloro</span></div><div class="pt-cell gas-noble" title="Argón — Z=18, grupo 18, período 3"><span class="z">18</span><strong>Ar</strong><span class="name">Argón</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Potasio — Z=19, grupo 1, período 4"><span class="z">19</span><strong>K</strong><span class="name">Potasio</span></div><div class="pt-cell alcalinoterreo" title="Calcio — Z=20, grupo 2, período 4"><span class="z">20</span><strong>Ca</strong><span class="name">Calcio</span></div><div class="pt-cell transicion" title="Escandio — Z=21, grupo 3, período 4"><span class="z">21</span><strong>Sc</strong><span class="name">Escandio</span></div><div class="pt-cell transicion" title="Titanio — Z=22, grupo 4, período 4"><span class="z">22</span><strong>Ti</strong><span class="name">Titanio</span></div><div class="pt-cell transicion" title="Vanadio — Z=23, grupo 5, período 4"><span class="z">23</span><strong>V</strong><span class="name">Vanadio</span></div><div class="pt-cell transicion" title="Cromo — Z=24, grupo 6, período 4"><span class="z">24</span><strong>Cr</strong><span class="name">Cromo</span></div><div class="pt-cell transicion" title="Manganeso — Z=25, grupo 7, período 4"><span class="z">25</span><strong>Mn</strong><span class="name">Manganeso</span></div><div class="pt-cell transicion" title="Hierro — Z=26, grupo 8, período 4"><span class="z">26</span><strong>Fe</strong><span class="name">Hierro</span></div><div class="pt-cell transicion" title="Cobalto — Z=27, grupo 9, período 4"><span class="z">27</span><strong>Co</strong><span class="name">Cobalto</span></div><div class="pt-cell transicion" title="Níquel — Z=28, grupo 10, período 4"><span class="z">28</span><strong>Ni</strong><span class="name">Níquel</span></div><div class="pt-cell transicion" title="Cobre — Z=29, grupo 11, período 4"><span class="z">29</span><strong>Cu</strong><span class="name">Cobre</span></div><div class="pt-cell transicion" title="Zinc — Z=30, grupo 12, período 4"><span class="z">30</span><strong>Zn</strong><span class="name">Zinc</span></div><div class="pt-cell metal" title="Galio — Z=31, grupo 13, período 4"><span class="z">31</span><strong>Ga</strong><span class="name">Galio</span></div><div class="pt-cell metaloide" title="Germanio — Z=32, grupo 14, período 4"><span class="z">32</span><strong>Ge</strong><span class="name">Germanio</span></div><div class="pt-cell metaloide" title="Arsénico — Z=33, grupo 15, período 4"><span class="z">33</span><strong>As</strong><span class="name">Arsénico</span></div><div class="pt-cell no-metal" title="Selenio — Z=34, grupo 16, período 4"><span class="z">34</span><strong>Se</strong><span class="name">Selenio</span></div><div class="pt-cell halogeno" title="Bromo — Z=35, grupo 17, período 4"><span class="z">35</span><strong>Br</strong><span class="name">Bromo</span></div><div class="pt-cell gas-noble" title="Kriptón — Z=36, grupo 18, período 4"><span class="z">36</span><strong>Kr</strong><span class="name">Kriptón</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Rubidio — Z=37, grupo 1, período 5"><span class="z">37</span><strong>Rb</strong><span class="name">Rubidio</span></div><div class="pt-cell alcalinoterreo" title="Estroncio — Z=38, grupo 2, período 5"><span class="z">38</span><strong>Sr</strong><span class="name">Estroncio</span></div><div class="pt-cell transicion" title="Itrio — Z=39, grupo 3, período 5"><span class="z">39</span><strong>Y</strong><span class="name">Itrio</span></div><div class="pt-cell transicion" title="Circonio — Z=40, grupo 4, período 5"><span class="z">40</span><strong>Zr</strong><span class="name">Circonio</span></div><div class="pt-cell transicion" title="Niobio — Z=41, grupo 5, período 5"><span class="z">41</span><strong>Nb</strong><span class="name">Niobio</span></div><div class="pt-cell transicion" title="Molibdeno — Z=42, grupo 6, período 5"><span class="z">42</span><strong>Mo</strong><span class="name">Molibdeno</span></div><div class="pt-cell transicion" title="Tecnecio — Z=43, grupo 7, período 5"><span class="z">43</span><strong>Tc</strong><span class="name">Tecnecio</span></div><div class="pt-cell transicion" title="Rutenio — Z=44, grupo 8, período 5"><span class="z">44</span><strong>Ru</strong><span class="name">Rutenio</span></div><div class="pt-cell transicion" title="Rodio — Z=45, grupo 9, período 5"><span class="z">45</span><strong>Rh</strong><span class="name">Rodio</span></div><div class="pt-cell transicion" title="Paladio — Z=46, grupo 10, período 5"><span class="z">46</span><strong>Pd</strong><span class="name">Paladio</span></div><div class="pt-cell transicion" title="Plata — Z=47, grupo 11, período 5"><span class="z">47</span><strong>Ag</strong><span class="name">Plata</span></div><div class="pt-cell transicion" title="Cadmio — Z=48, grupo 12, período 5"><span class="z">48</span><strong>Cd</strong><span class="name">Cadmio</span></div><div class="pt-cell metal" title="Indio — Z=49, grupo 13, período 5"><span class="z">49</span><strong>In</strong><span class="name">Indio</span></div><div class="pt-cell metal" title="Estaño — Z=50, grupo 14, período 5"><span class="z">50</span><strong>Sn</strong><span class="name">Estaño</span></div><div class="pt-cell metaloide" title="Antimonio — Z=51, grupo 15, período 5"><span class="z">51</span><strong>Sb</strong><span class="name">Antimonio</span></div><div class="pt-cell metaloide" title="Telurio — Z=52, grupo 16, período 5"><span class="z">52</span><strong>Te</strong><span class="name">Telurio</span></div><div class="pt-cell halogeno" title="Yodo — Z=53, grupo 17, período 5"><span class="z">53</span><strong>I</strong><span class="name">Yodo</span></div><div class="pt-cell gas-noble" title="Xenón — Z=54, grupo 18, período 5"><span class="z">54</span><strong>Xe</strong><span class="name">Xenón</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Cesio — Z=55, grupo 1, período 6"><span class="z">55</span><strong>Cs</strong><span class="name">Cesio</span></div><div class="pt-cell alcalinoterreo" title="Bario — Z=56, grupo 2, período 6"><span class="z">56</span><strong>Ba</strong><span class="name">Bario</span></div><div class="pt-cell empty"></div><div class="pt-cell transicion" title="Hafnio — Z=72, grupo 4, período 6"><span class="z">72</span><strong>Hf</strong><span class="name">Hafnio</span></div><div class="pt-cell transicion" title="Tantalio — Z=73, grupo 5, período 6"><span class="z">73</span><strong>Ta</strong><span class="name">Tantalio</span></div><div class="pt-cell transicion" title="Wolframio — Z=74, grupo 6, período 6"><span class="z">74</span><strong>W</strong><span class="name">Wolframio</span></div><div class="pt-cell transicion" title="Renio — Z=75, grupo 7, período 6"><span class="z">75</span><strong>Re</strong><span class="name">Renio</span></div><div class="pt-cell transicion" title="Osmio — Z=76, grupo 8, período 6"><span class="z">76</span><strong>Os</strong><span class="name">Osmio</span></div><div class="pt-cell transicion" title="Iridio — Z=77, grupo 9, período 6"><span class="z">77</span><strong>Ir</strong><span class="name">Iridio</span></div><div class="pt-cell transicion" title="Platino — Z=78, grupo 10, período 6"><span class="z">78</span><strong>Pt</strong><span class="name">Platino</span></div><div class="pt-cell transicion" title="Oro — Z=79, grupo 11, período 6"><span class="z">79</span><strong>Au</strong><span class="name">Oro</span></div><div class="pt-cell transicion" title="Mercurio — Z=80, grupo 12, período 6"><span class="z">80</span><strong>Hg</strong><span class="name">Mercurio</span></div><div class="pt-cell metal" title="Talio — Z=81, grupo 13, período 6"><span class="z">81</span><strong>Tl</strong><span class="name">Talio</span></div><div class="pt-cell metal" title="Plomo — Z=82, grupo 14, período 6"><span class="z">82</span><strong>Pb</strong><span class="name">Plomo</span></div><div class="pt-cell metal" title="Bismuto — Z=83, grupo 15, período 6"><span class="z">83</span><strong>Bi</strong><span class="name">Bismuto</span></div><div class="pt-cell metal" title="Polonio — Z=84, grupo 16, período 6"><span class="z">84</span><strong>Po</strong><span class="name">Polonio</span></div><div class="pt-cell halogeno" title="Astato — Z=85, grupo 17, período 6"><span class="z">85</span><strong>At</strong><span class="name">Astato</span></div><div class="pt-cell gas-noble" title="Radón — Z=86, grupo 18, período 6"><span class="z">86</span><strong>Rn</strong><span class="name">Radón</span></div></div><div class="pt-row"><div class="pt-cell alcalino" title="Francio — Z=87, grupo 1, período 7"><span class="z">87</span><strong>Fr</strong><span class="name">Francio</span></div><div class="pt-cell alcalinoterreo" title="Radio — Z=88, grupo 2, período 7"><span class="z">88</span><strong>Ra</strong><span class="name">Radio</span></div><div class="pt-cell empty"></div><div class="pt-cell transicion" title="Rutherfordio — Z=104, grupo 4, período 7"><span class="z">104</span><strong>Rf</strong><span class="name">Rutherfordio</span></div><div class="pt-cell transicion" title="Dubnio — Z=105, grupo 5, período 7"><span class="z">105</span><strong>Db</strong><span class="name">Dubnio</span></div><div class="pt-cell transicion" title="Seaborgio — Z=106, grupo 6, período 7"><span class="z">106</span><strong>Sg</strong><span class="name">Seaborgio</span></div><div class="pt-cell transicion" title="Bohrio — Z=107, grupo 7, período 7"><span class="z">107</span><strong>Bh</strong><span class="name">Bohrio</span></div><div class="pt-cell transicion" title="Hassio — Z=108, grupo 8, período 7"><span class="z">108</span><strong>Hs</strong><span class="name">Hassio</span></div><div class="pt-cell transicion" title="Meitnerio — Z=109, grupo 9, período 7"><span class="z">109</span><strong>Mt</strong><span class="name">Meitnerio</span></div><div class="pt-cell transicion" title="Darmstadtio — Z=110, grupo 10, período 7"><span class="z">110</span><strong>Ds</strong><span class="name">Darmstadtio</span></div><div class="pt-cell transicion" title="Roentgenio — Z=111, grupo 11, período 7"><span class="z">111</span><strong>Rg</strong><span class="name">Roentgenio</span></div><div class="pt-cell transicion" title="Copernicio — Z=112, grupo 12, período 7"><span class="z">112</span><strong>Cn</strong><span class="name">Copernicio</span></div><div class="pt-cell metal" title="Nihonio — Z=113, grupo 13, período 7"><span class="z">113</span><strong>Nh</strong><span class="name">Nihonio</span></div><div class="pt-cell metal" title="Flerovio — Z=114, grupo 14, período 7"><span class="z">114</span><strong>Fl</strong><span class="name">Flerovio</span></div><div class="pt-cell metal" title="Moscovio — Z=115, grupo 15, período 7"><span class="z">115</span><strong>Mc</strong><span class="name">Moscovio</span></div><div class="pt-cell metal" title="Livermorio — Z=116, grupo 16, período 7"><span class="z">116</span><strong>Lv</strong><span class="name">Livermorio</span></div><div class="pt-cell halogeno" title="Tenesino — Z=117, grupo 17, período 7"><span class="z">117</span><strong>Ts</strong><span class="name">Tenesino</span></div><div class="pt-cell gas-noble" title="Oganesón — Z=118, grupo 18, período 7"><span class="z">118</span><strong>Og</strong><span class="name">Oganesón</span></div></div></div>
<div class="fblock"><div class="f-label">Lantánidos</div><div class="f-row"><div class="pt-cell lantanido" title="Lantano — Z=57, grupo f-block, período 6"><span class="z">57</span><strong>La</strong><span class="name">Lantano</span></div><div class="pt-cell lantanido" title="Cerio — Z=58, grupo f-block, período 6"><span class="z">58</span><strong>Ce</strong><span class="name">Cerio</span></div><div class="pt-cell lantanido" title="Praseodimio — Z=59, grupo f-block, período 6"><span class="z">59</span><strong>Pr</strong><span class="name">Praseodimio</span></div><div class="pt-cell lantanido" title="Neodimio — Z=60, grupo f-block, período 6"><span class="z">60</span><strong>Nd</strong><span class="name">Neodimio</span></div><div class="pt-cell lantanido" title="Prometio — Z=61, grupo f-block, período 6"><span class="z">61</span><strong>Pm</strong><span class="name">Prometio</span></div><div class="pt-cell lantanido" title="Samario — Z=62, grupo f-block, período 6"><span class="z">62</span><strong>Sm</strong><span class="name">Samario</span></div><div class="pt-cell lantanido" title="Europio — Z=63, grupo f-block, período 6"><span class="z">63</span><strong>Eu</strong><span class="name">Europio</span></div><div class="pt-cell lantanido" title="Gadolinio — Z=64, grupo f-block, período 6"><span class="z">64</span><strong>Gd</strong><span class="name">Gadolinio</span></div><div class="pt-cell lantanido" title="Terbio — Z=65, grupo f-block, período 6"><span class="z">65</span><strong>Tb</strong><span class="name">Terbio</span></div><div class="pt-cell lantanido" title="Disprosio — Z=66, grupo f-block, período 6"><span class="z">66</span><strong>Dy</strong><span class="name">Disprosio</span></div><div class="pt-cell lantanido" title="Holmio — Z=67, grupo f-block, período 6"><span class="z">67</span><strong>Ho</strong><span class="name">Holmio</span></div><div class="pt-cell lantanido" title="Erbio — Z=68, grupo f-block, período 6"><span class="z">68</span><strong>Er</strong><span class="name">Erbio</span></div><div class="pt-cell lantanido" title="Tulio — Z=69, grupo f-block, período 6"><span class="z">69</span><strong>Tm</strong><span class="name">Tulio</span></div><div class="pt-cell lantanido" title="Iterbio — Z=70, grupo f-block, período 6"><span class="z">70</span><strong>Yb</strong><span class="name">Iterbio</span></div><div class="pt-cell lantanido" title="Lutecio — Z=71, grupo f-block, período 6"><span class="z">71</span><strong>Lu</strong><span class="name">Lutecio</span></div></div><div class="f-label">Actínidos</div><div class="f-row"><div class="pt-cell actinido" title="Actinio — Z=89, grupo f-block, período 7"><span class="z">89</span><strong>Ac</strong><span class="name">Actinio</span></div><div class="pt-cell actinido" title="Torio — Z=90, grupo f-block, período 7"><span class="z">90</span><strong>Th</strong><span class="name">Torio</span></div><div class="pt-cell actinido" title="Protactinio — Z=91, grupo f-block, período 7"><span class="z">91</span><strong>Pa</strong><span class="name">Protactinio</span></div><div class="pt-cell actinido" title="Uranio — Z=92, grupo f-block, período 7"><span class="z">92</span><strong>U</strong><span class="name">Uranio</span></div><div class="pt-cell actinido" title="Neptunio — Z=93, grupo f-block, período 7"><span class="z">93</span><strong>Np</strong><span class="name">Neptunio</span></div><div class="pt-cell actinido" title="Plutonio — Z=94, grupo f-block, período 7"><span class="z">94</span><strong>Pu</strong><span class="name">Plutonio</span></div><div class="pt-cell actinido" title="Americio — Z=95, grupo f-block, período 7"><span class="z">95</span><strong>Am</strong><span class="name">Americio</span></div><div class="pt-cell actinido" title="Curio — Z=96, grupo f-block, período 7"><span class="z">96</span><strong>Cm</strong><span class="name">Curio</span></div><div class="pt-cell actinido" title="Berkelio — Z=97, grupo f-block, período 7"><span class="z">97</span><strong>Bk</strong><span class="name">Berkelio</span></div><div class="pt-cell actinido" title="Californio — Z=98, grupo f-block, período 7"><span class="z">98</span><strong>Cf</strong><span class="name">Californio</span></div><div class="pt-cell actinido" title="Einsteinio — Z=99, grupo f-block, período 7"><span class="z">99</span><strong>Es</strong><span class="name">Einsteinio</span></div><div class="pt-cell actinido" title="Fermio — Z=100, grupo f-block, período 7"><span class="z">100</span><strong>Fm</strong><span class="name">Fermio</span></div><div class="pt-cell actinido" title="Mendelevio — Z=101, grupo f-block, período 7"><span class="z">101</span><strong>Md</strong><span class="name">Mendelevio</span></div><div class="pt-cell actinido" title="Nobelio — Z=102, grupo f-block, período 7"><span class="z">102</span><strong>No</strong><span class="name">Nobelio</span></div><div class="pt-cell actinido" title="Lawrencio — Z=103, grupo f-block, período 7"><span class="z">103</span><strong>Lr</strong><span class="name">Lawrencio</span></div></div></div></div>
<div class="legend"><span class="legend-item alcalino">Alcalinos</span><span class="legend-item alcalinoterreo">Alcalinotérreos</span><span class="legend-item transicion">Metales de transición</span><span class="legend-item metal">Otros metales</span><span class="legend-item metaloide">Metaloides</span><span class="legend-item no-metal">No metales</span><span class="legend-item halogeno">Halógenos</span><span class="legend-item gas-noble">Gases nobles</span><span class="legend-item lantanido">Lantánidos</span><span class="legend-item actinido">Actínidos</span></div>

</section><section id="fisica" class="module module-fisica"><h2>⚡ Física</h2>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Física y Medición</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia las magnitudes físicas y las unidades estandarizadas del Sistema Internacional (SI) para cuantificar fenómenos naturales.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Magnitudes Fundamentales:</strong> Longitud ($m$), Masa ($kg$), Tiempo ($s$).</p>
<p>• <strong>Magnitudes Derivadas:</strong> Resultan de combinar las fundamentales (ej: Velocidad en $m/s$, Fuerza en $N$).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Sistema Internacional (SI):</strong> Base unificada de medición ($m, kg, s$).</li>
<li><strong>Análisis Dimensional:</strong> Comprobación de consistencia de unidades en ambos lados de una igualdad.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Verificar si la unidad de la velocidad ($v = d / t$) es consistente.</p>
<p>• <strong>Paso 1 (Identificar el concepto):</strong> La velocidad resulta del cociente entre distancia y tiempo.</p>
<p>• <strong>Paso 2 (Reconocer elementos):</strong> La distancia se mide en metros ($m$) y el tiempo en segundos ($s$).</p>
<p>• <strong>Paso 3 (Relacionar):</strong> $\text{Unidad de } v = \frac{\text{metros}}{\text{segundos}} = \text{m/s}$.</p>
<p>• <strong>Paso 4 (Explicar conclusión):</strong> La unidad $m/s$ es dimensionalmente válida. Si en un cálculo de velocidad obtienes $kg/s$, hay un error previo.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Sabiendo que la densidad se define como $\rho = m / V$, expresá sus unidades en el Sistema Internacional.</p>
<p><strong>✅ Solución:</strong> La masa se mide en $kg$ y el volumen en $m^3$; por lo tanto, la unidad es $kg/m^3$.</p>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Magnitudes Escalares, Vectoriales y Trigonometría</h3>
<p><strong>¿Qué es?</strong></p>
<p>Representa magnitudes físicas que poseen magnitud, dirección y sentido mediante vectores y trigonometría.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Escalar:</strong> Magnitud representada solo por un número y su unidad (temperatura, masa).</p>
<p>• <strong>Vectorial:</strong> Requiere magnitud, dirección y sentido (fuerza, velocidad).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Componente X:</strong> $v_x = M \cdot \cos\theta$.</li>
<li><strong>Componente Y:</strong> $v_y = M \cdot \sin\theta$.</li>
<li><strong>Módulo:</strong> $M = \sqrt{v_x^2 + v_y^2}$.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Hallar las componentes del vector fuerza $F = 10\text{ N}$ que actúa a $\theta = 30^\circ$ sobre la horizontal.</p>
<p>• <strong>Paso 1 (Identificar datos):</strong> Módulo $M = 10\text{ N}$, ángulo $\theta = 30^\circ$.</p>
<p>• <strong>Paso 2 (Elegir fórmulas):</strong> $F_x = M \cdot \cos(30^\circ)$ y $F_y = M \cdot \sin(30^\circ)$.</p>
<p>• <strong>Paso 3 (Reemplazar y calcular):</strong>
$F_x = 10 \cdot 0.866 = 8.66\text{ N}$
$F_y = 10 \cdot 0.5 = 5.0\text{ N}$</p>
<p>• <strong>Paso 4 (Resultado):</strong> El vector expresado en componentes es $(8.66\text{ N}, 5.0\text{ N})$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Calculá la componente horizontal $v_x$ de una velocidad de $20\text{ m/s}$ inclinada a $60^\circ$ respecto a la horizontal.</p>
<p><strong>✅ Solución:</strong> $v_x = 20 \cdot \cos(60^\circ) = 20 \cdot 0.5 = 10\text{ m/s}$.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Cinemática Básica (MRU y MRUV)</h3>
<p><strong>¿Qué es?</strong></p>
<p>Describe el movimiento de los cuerpos en función del tiempo sin considerar las causas que lo producen.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>MRU:</strong> Velocidad constante ($a = 0$). Fórmula: $x = x_0 + v \cdot t$.</p>
<p>• <strong>MRUV:</strong> Aceleración constante ($a \neq 0$). Fórmula: $v = v_0 + a \cdot t$ y $x = x_0 + v_0 t + \frac{1}{2}a t^2$.</p>
<p><strong>⚠️ Interpretación gráfica:</strong> En un gráfico posición-tiempo ($x$-$t$), la pendiente es la velocidad; en un gráfico velocidad-tiempo ($v$-$t$), la pendiente representa la aceleración y el área bajo la curva es el desplazamiento.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>MRU:</strong> $v = \text{constante} \quad | \quad x = x_0 + v \cdot t$.</li>
<li><strong>MRUV:</strong> $a = \text{constante} \quad | \quad v = v_0 + a \cdot t \quad | \quad x = x_0 + v_0 t + \frac{1}{2}a t^2$.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Un móvil parte del reposo ($v_0 = 0$) y alcanza una velocidad de $20\text{ m/s}$ en $5\text{ s}$. Calcular su aceleración.</p>
<p>• <strong>Paso 1 (Datos):</strong> $v_0 = 0\text{ m/s}$, $v = 20\text{ m/s}$, $t = 5\text{ s}$.</p>
<p>• <strong>Paso 2 (Fórmula):</strong> $a = \frac{v - v_0}{t}$.</p>
<p>• <strong>Paso 3 (Reemplazar y resolver):</strong> $a = \frac{20 - 0}{5} = 4\text{ m/s}^2$.</p>
<p>• <strong>Paso 4 (Resultado):</strong> La aceleración del móvil es de $4\text{ m/s}^2$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Utilizando la aceleración calculada de $4\text{ m/s}^2$, calculá la distancia recorrida en esos $5\text{ s}$ partiendo del reposo.</p>
<p><strong>✅ Solución:</strong> $x = 0 + (0 \cdot 5) + \frac{1}{2}(4)(5^2) = \frac{1}{2}(4)(25) = 50\text{ m}$.</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Leyes de Newton, Trabajo y Conservación de la Energía</h3>
<p><strong>¿Qué es?</strong></p>
<p>Explica la causa del movimiento mediante fuerzas y cuantifica la transferencia y conservación de la energía.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>2ª Ley de Newton:</strong> $F = m \cdot a$.</p>
<p>• <strong>Trabajo ($W$):</strong> $W = F \cdot d \cdot \cos\theta$. <strong>Potencia ($P$):</strong> $P = W / t$.</p>
<p>• <strong>Conservación:</strong> Sin rozamiento, $E_{mecanica} = E_c + E_p = \text{constante}$.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Leyes de Newton:</strong> 1ª Inercia | 2ª $F = ma$ | 3ª Acción-Reacción.</li>
<li><strong>Energía Cinética / Potencial:</strong> $E_c = \frac{1}{2}m v^2$ | $E_p = m \cdot g \cdot h$.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Calcular la energía potencial gravitatoria de un objeto de $1\text{ kg}$ situado a $5\text{ m}$ de altura ($g = 9.8\text{ m/s}^2$).</p>
<p>• <strong>Paso 1 (Datos):</strong> $m = 1\text{ kg}$, $g = 9.8\text{ m/s}^2$, $h = 5\text{ m}$.</p>
<p>• <strong>Paso 2 (Fórmula):</strong> $E_p = m \cdot g \cdot h$.</p>
<p>• <strong>Paso 3 (Resolver):</strong> $E_p = 1 \cdot 9.8 \cdot 5 = 49\text{ Joules}$.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> Al caer al suelo sin fricción, toda esa $E_p$ se transforma en $49\text{ J}$ de Energía Cinética ($E_c$).</p>
<p><strong>✏️ Practicá</strong></p>
<p>¿Qué fuerza neta se necesita aplicar a una masa de $2\text{ kg}$ para que acelere a $3\text{ m/s}^2$?</p>
<p><strong>✅ Solución:</strong> $F = m \cdot a = 2\text{ kg} \cdot 3\text{ m/s}^2 = 6\text{ N}$.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Hidrostática e Hidrodinámica</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia el comportamiento de los fluidos en reposo y en movimiento.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Presión Hidrostática Absoluta:</strong> $P = P_0 + \rho \cdot g \cdot h$ (donde $P_0$ es la presión atmosférica en la superficie).</p>
<p>• <strong>Principio de Pascal:</strong> La presión aplicada a un fluido encerrado se transmite con igual intensidad en todas direcciones.</p>
<p>• <strong>Principio de Arquímedes:</strong> Todo cuerpo sumergido experimenta un empuje vertical hacia arriba igual al peso del fluido desalojado ($E = \rho_{fluido} \cdot g \cdot V_{desalojado}$).</p>
<p><strong>⚠️ Aclaraciones de Hidrodinámica:</strong>
• <strong>Continuidad:</strong> En un flujo estacionario e incompresible, sin acumulación, el caudal se conserva ($Q = A_1 v_1 = A_2 v_2$).
• <strong>Bernoulli:</strong> La relación $P + \frac{1}{2}\rho v^2 + \rho g h = \text{cte}$ se aplica bajo condiciones ideales de flujo estacionario e incompresible a lo largo de una línea de corriente.
• <strong>Ejemplo en tuberías:</strong> Cuando un fluido circula por una tubería que se estrecha, su velocidad aumenta y, bajo determinadas condiciones, su presión disminuye.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Presión Absoluta:</strong> $P = P_0 + \rho \cdot g \cdot h$.</li>
<li><strong>Empuje:</strong> $E = \rho_{fluido} \cdot g \cdot V_{desalojado}$.</li>
<li><strong>Continuidad / Bernoulli:</strong> $A_1 v_1 = A_2 v_2 \quad | \quad P + \frac{1}{2}\rho v^2 + \rho g h = \text{constante}$.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Un buzo se encuentra sumergido a $10\text{ m}$ de profundidad en el mar ($\rho = 1025\text{ kg/m}^3$, $g = 9.8\text{ m/s}^2$). Si la presión en la superficie es $P_0 = 101325\text{ Pa}$, hallar la presión absoluta que soporta.</p>
<p>• <strong>Paso 1 (Datos):</strong> $P_0 = 101325\text{ Pa}$, $\rho = 1025\text{ kg/m}^3$, $g = 9.8\text{ m/s}^2$, $h = 10\text{ m}$.</p>
<p>• <strong>Paso 2 (Presión manométrica):</strong> $P_{man} = \rho \cdot g \cdot h = 1025 \cdot 9.8 \cdot 10 = 100450\text{ Pa}$.</p>
<p>• <strong>Paso 3 (Presión absoluta):</strong> $P = P_0 + P_{man} = 101325 + 100450 = 201775\text{ Pa}$.</p>
<p>• <strong>Paso 4 (Resultado):</strong> $P \approx 201.78\text{ kPa}$ (aproximadamente $2\text{ atm}$).</p>
<p><strong>✏️ Practicá</strong></p>
<p>Un objeto de volumen $V = 0.02\text{ m}^3$ se sumerge completamente en agua ($\rho = 1000\text{ kg/m}^3$). Calculá el empuje que experimenta.</p>
<p><strong>✅ Solución:</strong> $E = \rho \cdot g \cdot V = 1000\text{ kg/m}^3 \cdot 9.8\text{ m/s}^2 \cdot 0.02\text{ m}^3 = 196\text{ N}$.</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Viscosidad, Ley de Poiseuille y Transporte</h3>
<p><strong>¿Qué es?</strong></p>
<p>Describe el flujo de fluidos reales considerando la fricción interna y los mecanismos moleculares de transporte.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Ley de Poiseuille:</strong> Se aplica al flujo laminar de un fluido newtoniano por un tubo cilíndrico: $Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L}$. El caudal depende fuertemente del radio ($Q \propto r^4$).</p>
<p>• <strong>Ley de Fick:</strong> El flujo de difusión es proporcional al gradiente de concentración ($J = -D \cdot \frac{\Delta C}{\Delta x}$).</p>
<p><strong>⚠️ Correcciones de transporte:</strong>
• <strong>Ósmosis:</strong> Existe un movimiento neto de agua a través de una membrana semipermeable hacia el lado con mayor concentración efectiva de solutos, bajo determinadas condiciones.
• <strong>Fenómenos de transporte:</strong> Los fenómenos de transporte se relacionan mediante gradientes, flujos, difusión, convección, viscosidad y sedimentación (la viscosidad es una propiedad del fluido, no una etapa posterior a la difusión).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Poiseuille:</strong> Caudal en tubos proporcional al radio a la cuarta potencia ($r^4$).</li>
<li><strong>Difusión (Fick):</strong> Transporte pasivo a favor de gradiente de concentración.</li>
<li><strong>Ósmosis:</strong> Movimiento neto de solvente a través de membrana semipermeable.</li>
</ul>
<p><strong>🧮 Ejemplo conceptual</strong></p>
<p><strong>Enunciado:</strong> ¿Cómo impacta reducir a la mitad el radio de un conducto según Poiseuille?</p>
<p>• <strong>Paso 1:</strong> La relación del caudal con el radio es de cuarta potencia ($r^4$).</p>
<p>• <strong>Paso 2:</strong> Si el radio pasa a ser $r/2$, el factor en el caudal es $(1/2)^4 = 1/16$.</p>
<p>• <strong>Paso 3 (Conclusión):</strong> El caudal se reduce a la dieciseisava parte de su valor original.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar qué mecanismo de transporte es más rápido a distancias grandes: ¿la difusión pura o la convección de un fluido completo?</p>
<p><strong>✅ Solución:</strong> La convección, ya que desplaza la masa completa del fluido impulsada por trabajo mecánico (ej: bombeo).</p>
</section><section id="biologia" class="module module-biologia"><h2>🧬 Biología</h2>
<p><strong>🟢 RECONOCER</strong></p>
<h3>La Célula: Estructura y Organelos</h3>
<p><strong>¿Qué es?</strong></p>
<p>Describe la unidad fundamental de los seres vivos y las funciones biológicas de sus componentes subcelulares.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Procariota:</strong> Célula sin núcleo delimitado por membrana (ej: bacterias).</p>
<p>• <strong>Eucariota:</strong> Célula con núcleo organizado y organelos membranosos especializados.</p>
<p>• <strong>Núcleo:</strong> Contiene y resguarda el material genético.</p>
<p>• <strong>Mitocondria:</strong> Organela encargada de la producción de energía (ATP).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Estructura celular:</strong> Membrana plasmática, Citoplasma, Material genético.</li>
<li><strong>Sistemas membranosos:</strong> Retículo Endoplasmático (síntesis) $\to$ Aparato de Golgi (empaquetado y envío).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Identificar qué organela se desarrollará en mayor proporción en células con alta demanda energética (como las células musculares).</p>
<p>• <strong>Paso 1 (Identificar concepto):</strong> La demanda energética requiere síntesis masiva de ATP.</p>
<p>• <strong>Paso 2 (Reconocer elementos):</strong> La organela especializada en la respiración aeróbica y obtención de ATP es la mitocondria.</p>
<p>• <strong>Paso 3 (Relacionar):</strong> Estructuras con mayor trabajo mecánico consumen más ATP $\to$ requieren mayor densidad mitocondrial.</p>
<p>• <strong>Paso 4 (Explicar conclusión):</strong> Las células musculares poseen abundante cantidad de mitocondrias en su citoplasma.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar qué organela celular es la responsable directa del ensamblado de proteínas a partir de la información genética.</p>
<p><strong>✅ Solución:</strong> Los ribosomas.</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Metabolismo Energético: Respiración Celular y Fotosíntesis</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia los procesos bioquímicos mediante los cuales las células transforman y obtienen energía química útil.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Respiración Celular Aeróbica:</strong> Ocurre en tres fases principales: Glucólisis (citoplasma), Ciclo de Krebs (matriz mitocondrial) y Cadena respiratoria / Fosforilación oxidativa (membrana interna mitocondrial).</p>
<p>• <strong>Fotosíntesis:</strong> Transforma energía lumínica en energía química sintetizando nutrientes en los cloroplastos.</p>
<p><strong>⚠️ Modificación conceptual precisa:</strong> La respiración celular oxida nutrientes, como la glucosa, y produce ATP (en lugar de la metáfora simplificada de &quot;quemar glucosa&quot;).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Respiración Celular:</strong> Oxidación de glucosa $\to$ Glucólisis $\to$ Krebs $\to$ Cadena respiratoria $\to$ Producción de ATP.</li>
<li><strong>Fotosíntesis:</strong> Etapa fotoquímica (captación de luz en tilacoides) $\to$ Ciclo de Calvin (fijación de $CO_2$ en estroma).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Explicar el rol del oxígeno gaseoso ($O_2$) en la respiración celular aeróbica.</p>
<p>• <strong>Paso 1 (Identificar la fase):</strong> Ocurre en la membrana interna de la mitocondria durante la Cadena Respiratoria.</p>
<p>• <strong>Paso 2 (Reconocer su función):</strong> El $O_2$ actúa como el aceptor final de electrones e hidrógenos.</p>
<p>• <strong>Paso 3 (Relacionar producto):</strong> Al aceptar electrones y protones, el oxígeno se reduce formando agua ($H_2O$).</p>
<p>• <strong>Paso 4 (Conclusión):</strong> Sin oxígeno, la cadena de transporte se bloquea y la producción eficiente de ATP se detiene.</p>
<p><strong>✏️ Practicá</strong></p>
<p>¿En qué región concreta de la célula eucariota se lleva a cabo la Glucólisis?</p>
<p><strong>✅ Solución:</strong> En el citoplasma (o citosol).</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Ciclo Celular: Mitosis y Meiosis</h3>
<p><strong>¿Qué es?</strong></p>
<p>Comprende los mecanismos de división nuclear y celular para la reproducción de tejidos o la formación de gametos.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Fases ordenadas de la división:</strong> Profase, Metafase, Anafase, Telofase.</p>
<p><strong>⚠️ Modificaciones conceptuales precisas:</strong>
• <strong>Mitosis:</strong> Forma dos células hijas con el mismo número de cromosomas y, en general, la misma información genética.
• <strong>Meiosis:</strong> Genera gametos genéticamente diversos mediante recombinación (crossing-over) y distribución independiente de cromosomas.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Mitosis:</strong> Célula $2n \to 2$ células $2n$ (Crecimiento y renovación tisular).</li>
<li><strong>Meiosis:</strong> Célula $2n \to 4$ gametos $n$ (Reducción cromosómica y diversidad genética).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Comparar la dotación cromosómica de una célula de la piel y un espermatozoide en una especie con $2n = 46$.</p>
<p>• <strong>Paso 1 (Identificar proceso de origen):</strong> Célula de piel $\to$ Mitosis; Espermatozoide $\to$ Meiosis.</p>
<p>• <strong>Paso 2 (Evaluar ploidía):</strong> La célula somática mantiene la dotación diploide ($2n$); la germinal es haploide ($n$).</p>
<p>• <strong>Paso 3 (Calcular valores):</strong> Piel $= 46$ cromosomas; Espermatozoide $= 46 / 2 = 23$ cromosomas.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> La mitosis conserva la cantidad de cromosomas ($46$), mientras la meiosis la reduce a la mitad ($23$).</p>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar en qué fase específica de la división celular los cromosomas se alinean en el plano ecuatorial de la célula.</p>
<p><strong>✅ Solución:</strong> En la Metafase.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Genética, Genoma y Herencia Mendelia</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia los mecanismos de transmisión de la información hereditaria y la expresión del genotipo en el fenotipo.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Alelo:</strong> Variante posible de un gen en un locus determinado.</p>
<p>• <strong>Genotipo / Fenotipo:</strong> Genotipo es la combinación alélica; fenotipo es la característica observable.</p>
<p><strong>⚠️ Modificaciones conceptuales precisas:</strong>
• <strong>Genoma:</strong> Conjunto completo del material genético de un organismo.
• <strong>Gen:</strong> Segmento de ADN que contiene información para producir un producto funcional, como un ARN o una proteína, según el caso.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Genotipo:</strong> Homocigota ($AA$ / $aa$) | Heterocigota ($Aa$).</li>
<li><strong>Cuadro de Punnett:</strong> Matriz probabilística para predecir proporciones genotípicas y fenotípicas.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Predecir las proporciones del cruce monohíbrido entre dos individuos heterocigotas ($Aa \times Aa$), donde el alelo $A$ es dominante (color rojo) y $a$ es recesivo (color blanco).</p>
<p>• <strong>Paso 1 (Gametos):</strong> Cada padre produce gametos $A$ ($50\%$) y $a$ ($50\%$).</p>
<p>• <strong>Paso 2 (Cruzamiento):</strong> Combinaciones posibles en el Cuadro de Punnett: $AA$, $Aa$, $Aa$, $aa$.</p>
<p>• <strong>Paso 3 (Proporción Genotípica):</strong> $25\%\text{ } AA$, $50\%\text{ } Aa$, $25\%\text{ } aa$ (Relación 1:2:1).</p>
<p>• <strong>Paso 4 (Proporción Fenotípica):</strong> $75\%$ de individuos con fenotipo dominante (rojo) y $25\%$ con fenotipo recesivo (blanco).</p>
<p><strong>✏️ Practicá</strong></p>
<p>Al cruzar un individuo homocigota recesivo ($aa$) con un heterocigota ($Aa$), ¿qué porcentaje de la descendencia se espera que exprese el fenotipo recesivo?</p>
<p><strong>✅ Solución:</strong> $50\%$ (combinaciones resultantes: $Aa$, $Aa$, $aa$, $aa$).</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Expresión Génica, Evolución y Clasificación Taxonómica</h3>
<p><strong>¿Qué es?</strong></p>
<p>Comprende el flujo de la información genética, los mecanismos de cambio evolutivo en poblaciones y la ordenación de la diversidad biológica.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Dogma Molecular:</strong> Replicación ($\text{ADN} \to \text{ADN}$) $\to$ Transcripción ($\text{ADN} \to \text{ARN}$) $\to$ Traducción ($\text{ARN} \to \text{Proteína}$).</p>
<p><strong>⚠️ Modificaciones conceptuales precisas:</strong>
• <strong>Traducción:</strong> Los codones especifican aminoácidos o señales de inicio y terminación durante la traducción.
• <strong>Evolución:</strong> La selección natural puede aumentar la frecuencia de variantes ventajosas en un determinado ambiente (evitando la simplificación de &quot;favorece al más fuerte&quot;).
• <strong>Taxonomía:</strong> Los organismos se clasifican en grandes grupos taxonómicos, como dominios y reinos, según características compartidas y relaciones evolutivas.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Flujo genético:</strong> ADN $\to$ ARNm (núcleo) $\to$ Proteína en ribosoma (código genético leído por codones).</li>
<li><strong>Evolución:</strong> Mutación (fuente de variabilidad) + Selección natural (frecuencia alélica diferencial).</li>
<li><strong>Taxonomía:</strong> Nomenclatura binomial (<em>Género especie</em>) y clasificación en dominios y reinos.</li>
</ul>
<p><strong>🧮 Ejemplo conceptual paso a paso</strong></p>
<p><strong>Enunciado:</strong> Explicar cómo un cambio puntual en el ADN (mutación) puede alterar una proteína.</p>
<p>• <strong>Paso 1:</strong> La mutación modifica una base nitrogenada en la secuencia del gen en el ADN.</p>
<p>• <strong>Paso 2:</strong> Durante la transcripción, la secuencia del ARNm copia ese cambio.</p>
<p>• <strong>Paso 3:</strong> Durante la traducción, el codón alterado puede especificar un aminoácido diferente.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> Al cambiar la secuencia de aminoácidos, la estructura y función de la proteína resultante pueden modificarse.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar cuál es la estructura formada por un triplete de bases nitrogenadas en el ARNm que especifica un aminoácido.</p>
<p><strong>✅ Solución:</strong> Un codón.</p>
</section><section id="matematica" class="module module-matematica"><h2>📐 Matemática</h2>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Base Numérica, Notación Científica y Proporciones</h3>
<p><strong>¿Qué es?</strong></p>
<p>Comprende las operaciones numéricas fundamentales, el manejo de escalas con notación científica y las relaciones de proporcionalidad.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Notación Científica:</strong> Expresa números mediante $a \times 10^n$ (donde $1 \le |a| &lt; 10$).</p>
<p>• <strong>Porcentaje:</strong> Razón que representa una fracción de 100 partes iguales.</p>
<p><strong>⚠️ Aclaración sobre Regla de Tres:</strong> La aplicación de la regla de tres simple supone que existe una relación de proporcionalidad estricta entre las magnitudes involucradas.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Operaciones base:</strong> Fracciones, potencias y raíces (operaciones inversas).</li>
<li><strong>Notación científica:</strong> $a \times 10^n$ (exponente negativo para números $&lt; 1$; positivo para números $&gt; 10$).</li>
<li><strong>Proporcionalidad:</strong> Directa (ambas crecen) | Inversa (una crece, la otra decrece).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Si $5\text{ análisis}$ cuestan $500$, suponiendo proporcionalidad estricta entre precio y cantidad, calcular el costo de $8\text{ análisis}$.</p>
<p>• <strong>Paso 1 (Identificar datos):</strong> $5\text{ unidades} \to $500$; buscamos el precio $x$ para $8\text{ unidades}$.</p>
<p>• <strong>Paso 2 (Elegir procedimiento):</strong> Regla de tres directa: $x = \frac{8 \cdot 500}{5}$.</p>
<p>• <strong>Paso 3 (Resolver):</strong> $x = \frac{4000}{5} = $800$.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> Los $8\text{ análisis}$ cuestan $800$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Expresá el número $0.000000045$ en notación científica.</p>
<p><strong>✅ Solución:</strong> $4.5 \times 10^{-8}$ (se desplaza la coma 8 lugares a la derecha).</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Ecuaciones, Despejes y Sistemas de Ecuaciones</h3>
<p><strong>¿Qué es?</strong></p>
<p>Aísla incógnitas en planteos algebraicos aplicando operaciones inversas a ambos lados de la igualdad.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Ecuación Lineal:</strong> Igualdad de primer grado resoluble por despeje directo.</p>
<p>• <strong>Ecuación Cuadrática:</strong> De la forma $ax^2 + bx + c = 0$, resoluble con la fórmula resolvente $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Despeje:</strong> Aplicar operaciones inversas manteniendo el equilibrio de la igualdad.</li>
<li><strong>Sistemas:</strong> Dos o más incógnitas que deben satisfacer simultáneamente varias ecuaciones.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Despejar la incógnita $x$ en la ecuación $2x + 3 = 11$.</p>
<p>• <strong>Paso 1 (Identificar estructura):</strong> La incógnita $x$ está multiplicada por $2$ y sumada a $3$.</p>
<p>• <strong>Paso 2 (Restar constante):</strong> Restamos $3$ a ambos lados: $2x = 11 - 3 \implies 2x = 8$.</p>
<p>• <strong>Paso 3 (Dividir coeficiente):</strong> Dividimos por $2$ a ambos lados: $x = \frac{8}{2} = 4$.</p>
<p>• <strong>Paso 4 (Verificación):</strong> Reemplazamos $x = 4 \implies 2(4) + 3 = 8 + 3 = 11$. La igualdad se cumple.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Resolvé la ecuación cuadrática $x^2 - 5x + 6 = 0$ identificando $a, b, c$ y aplicando la fórmula resolvente.</p>
<p><strong>✅ Solución:</strong> $a=1, b=-5, c=6 \implies x = \frac{5 \pm \sqrt{25 - 24}}{2} = \frac{5 \pm 1}{2}$. Las soluciones son $x_1 = 3$ y $x_2 = 2$.</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Funciones, Logaritmos, Probabilidad y Estadística</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia los modelos de relación entre variables, la cuantificación de eventos aleatorios y la inferencia a partir de datos.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Funciones Exponenciales y Logarítmicas:</strong> Las funciones exponenciales pueden modelar crecimientos o decrecimientos rápidos; el logaritmo es su función inversa y permite trabajar con escalas multiplicativas.</p>
<p>• <strong>Probabilidad:</strong> Un evento es un resultado o conjunto de resultados posibles dentro de un espacio muestral.</p>
<p><strong>⚠️ Definición de Prueba de Hipótesis:</strong> Una prueba de hipótesis evalúa si una diferencia observada es compatible con el azar bajo un determinado modelo estadístico.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Funciones:</strong> Lineal ($y=mx+b$) | Cuadrática ($y=ax^2+bx+c$) | Exponencial y Logarítmica.</li>
<li><strong>Probabilidad:</strong> $P(\text{Evento}) = \frac{\text{Casos favorables}}{\text{Casos posibles}}$ (en eventos equiprobables).</li>
<li><strong>Estadística:</strong> Descriptiva (resume datos con media/desvío) | Inferencia (prueba de hipótesis).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Calcular la probabilidad simple de obtener un número par al lanzar un dado justo de 6 caras.</p>
<p>• <strong>Paso 1 (Casos posibles):</strong> El espacio muestral es $\{1, 2, 3, 4, 5, 6\}$, por lo que hay 6 casos posibles.</p>
<p>• <strong>Paso 2 (Casos favorables):</strong> Los números pares son $\{2, 4, 6\}$, por lo que hay 3 casos favorables.</p>
<p>• <strong>Paso 3 (Aplicar fórmula):</strong> $P(\text{Par}) = \frac{3}{6} = \frac{1}{2} = 0.5$.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> La probabilidad es del $50\%$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Sabiendo que $10^2 = 100$, indicá el valor del logaritmo en base 10: $\log_{10}(100)$.</p>
<p><strong>✅ Solución:</strong> $\log_{10}(100) = 2$, ya que el logaritmo es la función inversa de la potencia.</p>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Cálculo: Derivada e Integral</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia las tasas de cambio instantáneas y la acumulación continua de cantidades descritas por funciones.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Derivada ($f'(x)$):</strong> Representa geométricamente la <em>pendiente de la recta tangente</em> a la curva en un punto o la <em>tasa de cambio instantánea</em> de la función.</p>
<p>• <strong>Integral Definida ($\int_{a}^{b} f(x)dx$):</strong> Representa geométricamente el <em>área acumulada bajo la curva</em> entre los límites $a$ y $b$.</p>
<p><strong>⚠️ Clarificación sobre Puntos Críticos:</strong> Si $f'(x) = 0$, se obtiene un punto crítico. Este puede corresponder a un máximo local, un mínimo local o a ninguno (como en un punto de silla con tangente horizontal); se necesitan otros criterios (como el signo de la derivada segunda) para determinarlo. Esto debe separarse del análisis de concavidad e inflexión.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Derivada:</strong> Pendiente de la recta tangente / Tasa de cambio instantánea $\to f'(x) = 0$ da puntos críticos.</li>
<li><strong>Integral:</strong> Operación inversa a la derivada $\to \int_{a}^{b} f(x)dx$ calcula el área bajo la curva.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Dada la función de posición $x(t) = t^2$ en metros, hallar la velocidad instantánea en $t = 3\text{ s}$ sabiendo que la derivada de $t^2$ es $2t$.</p>
<p>• <strong>Paso 1 (Identificar concepto):</strong> La velocidad instantánea es la derivada de la posición: $v(t) = x'(t)$.</p>
<p>• <strong>Paso 2 (Obtener la función derivada):</strong> $v(t) = 2t$.</p>
<p>• <strong>Paso 3 (Evaluar en el punto):</strong> $v(3) = 2(3) = 6\text{ m/s}$.</p>
<p>• <strong>Paso 4 (Conclusión):</strong> La pendiente de la recta tangente en $t = 3\text{ s}$ es $6$, lo que significa que la velocidad es de $6\text{ m/s}$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Dada $f(x) = x^3$, cuya derivada es $f'(x) = 3x^2$, hallá la pendiente de la recta tangente en $x = 2$.</p>
<p><strong>✅ Solución:</strong> $f'(2) = 3(2^2) = 3(4) = 12$.</p>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Álgebra Lineal, Teoría de Grafos y Optimización</h3>
<p><strong>¿Qué es?</strong></p>
<p>Procesa estructuras multidimensionales, representa redes de elementos interconectados y busca los valores óptimos de un sistema.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Vectores y Matrices:</strong> Listas y tablas organizadas de números para representar datos en múltiples dimensiones.</p>
<p>• <strong>PCA (Análisis de Componentes Principales):</strong> Técnica de álgebra lineal para reducir la dimensión de un conjunto de datos sin perder información relevante.</p>
<p>• <strong>Teoría de Grafos:</strong> Estructuras formadas por <strong>Nodos</strong> (elementos) y <strong>Aristas</strong> (conexiones) para representar redes de interacción.</p>
<p><strong>⚠️ Concepto de Optimización:</strong> La optimización puede utilizarse para encontrar máximos o mínimos de una función y también para ajustar modelos matemáticos a datos experimentales.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Álgebra Lineal:</strong> Operaciones con matrices $\to$ Reducción de dimensiones (PCA).</li>
<li><strong>Grafos:</strong> Nodos (puntos) + Aristas (líneas) $\to$ Representación de redes complejas.</li>
<li><strong>Optimización:</strong> Búsqueda de máximos/mínimos o ajuste de parámetros a datos reales.</li>
</ul>
<p><strong>🧮 Ejemplo conceptual paso a paso</strong></p>
<p><strong>Enunciado:</strong> Representar una red donde 3 personas (A, B, C) están conectadas si son amigas: A es amiga de B, y B es amiga de C.</p>
<p>• <strong>Paso 1 (Identificar Nodos):</strong> Los elementos son las 3 personas $\to$ Nodos = $\{A, B, C\}$.</p>
<p>• <strong>Paso 2 (Identificar Aristas):</strong> Las conexiones son las relaciones $\to$ Aristas = $\{(A,B), (B,C)\}$.</p>
<p>• <strong>Paso 3 (Conclusión):</strong> Se forma un grafo de 3 nodos y 2 aristas.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Si agregamos una amistad directa entre A y C en el ejemplo anterior, ¿cuántas aristas tendrá el grafo final?</p>
<p><strong>✅ Solución:</strong> Tendrá 3 aristas: $\{(A,B), (B,C), (A,C)\}$.</p>
</section><section id="programacion" class="module module-programacion"><h2>💻 Programación (Python)</h2>
<p><strong>🟢 RECONOCER</strong></p>
<h3>Algoritmos, Variables y Estructuras de Control</h3>
<p><strong>¿Qué es?</strong></p>
<p>Estudia el diseño de secuencias lógicas e inequívocas de pasos (algoritmos) para procesar datos y tomar decisiones en un lenguaje de programación.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Tipos de datos básicos:</strong> Enteros (`int`), Decimales (`float`), Texto (`str`) y Booleanos (`bool`).</p>
<p>• <strong>Condicionales (`if` / `else`):</strong> Permiten bifurcar el flujo de ejecución según el cumplimiento de una condición lógica.</p>
<p><strong>⚠️ Definición del Bucle `while`:</strong> El bucle `while` repite la ejecución de un bloque de código mientras una condición dada sea verdadera (a diferencia de `for`, que suele iterar sobre una colección o rango predefinido).</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Estructura general:</strong> Datos de entrada $\to$ Algoritmo $\to$ Resultado de salida.</li>
<li><strong>Bucles:</strong> `for` (iteración sobre colecciones) | `while` (repetición condicionada).</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso</strong></p>
<p><strong>Enunciado:</strong> Escribir un script que evalúe si una temperatura supera un valor de referencia.</p>
<pre><code class="language-python">temperatura = 38.0

if temperatura &gt; 37.5:
    print(&quot;Supera el valor de referencia&quot;)
else:
    print(&quot;No supera el valor de referencia&quot;)
</code></pre>
<p>• <strong>Resultado:</strong> Imprime <code>&quot;Supera el valor de referencia&quot;</code> porque $38.0 &gt; 37.5$.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Escribí una estructura `if` / `else` que verifique si una variable `temperatura` es mayor a $37.5$ y muestre `&quot;Fiebre&quot;` o `&quot;Normal&quot;`.</p>
<p><strong>✅ Solución:</strong></p>
<pre><code class="language-python">if temperatura &gt; 37.5:
    print(&quot;Fiebre&quot;)
else:
    print(&quot;Normal&quot;)
</code></pre>
<p><strong>🔴 RESOLVER</strong></p>
<h3>Colecciones, Búsqueda, Ordenamiento y Archivos</h3>
<p><strong>¿Qué es?</strong></p>
<p>Almacena conjuntos de datos estructurados en memoria y gestiona la lectura y escritura de archivos de datos externos.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Listas:</strong> Colecciones ordenadas de elementos modificables accesibles por índice numérico (`lista[0]`).</p>
<p>• <strong>Archivos CSV:</strong> Archivos de texto estructurados en filas y columnas; suelen utilizar comas como separador, aunque pueden emplear otros delimitadores como tabuladores o puntos y comas.</p>
<p><strong>⚠️ Modificaciones técnicas precisas:</strong>
• <strong>Diccionarios:</strong> En Python moderno, los diccionarios conservan el orden de inserción, pero se accede a sus elementos mediante claves, no mediante índices.
• <strong>Búsqueda y Ordenamiento:</strong> Una colección ordenada permite utilizar algoritmos de búsqueda eficientes, como la búsqueda binaria, cuando corresponde.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Colecciones:</strong> Listas (acceso por índice) | Diccionarios (acceso por clave).</li>
<li><strong>Lectura de archivos:</strong> Sentencia `with open(...)` para garantizar el cierre seguro del archivo.</li>
</ul>
<p><strong>🧮 Ejemplo resuelto paso a paso (Recorrer cadena y contar frecuencias)</strong></p>
<p><strong>Enunciado:</strong> Contar la frecuencia de cada carácter en una cadena de texto almacenando los resultados en un diccionario.</p>
<pre><code class="language-python">texto = &quot;PROGRAMACION&quot;
frecuencias = {}

for caracter in texto:
    frecuencias[caracter] = frecuencias.get(caracter, 0) + 1

print(frecuencias)
</code></pre>
<p>• <strong>Resultado:</strong> `{'G': 1, 'A': 3, 'T': 2, 'C': 1}`.</p>
<p><strong>✏️ Practicá</strong></p>
<p>Escribí el patrón de código seguro en Python para abrir y leer un archivo de texto llamado `&quot;datos.txt&quot;` utilizando `with open`.</p>
<p><strong>✅ Solución:</strong></p>
<pre><code class="language-python">with open(&quot;datos.txt&quot;, &quot;r&quot;, encoding=&quot;utf-8&quot;) as archivo:
    contenido = archivo.read()

print(contenido)
</code></pre>
<p><strong>🟡 ENTENDER</strong></p>
<h3>Funciones, Manejo de Errores, Git y GitHub</h3>
<p><strong>¿Qué es?</strong></p>
<p>Comprende la modularización del código en funciones reutilizables, la prevención de fallos en ejecución y el control de versiones colaborativo.</p>
<p><strong>🔎 Ideas clave</strong></p>
<p>• <strong>Funciones (`def`):</strong> Bloques de código modularizados que reciben parámetros de entrada y devuelven valores mediante `return`.</p>
<p>• <strong>Excepciones (`try` / `except`):</strong> Estructuras de control que previenen que el programa se detenga abruptamente ante errores inesperados.</p>
<p><strong>⚠️ Programación como herramienta universal:</strong> La programación es una herramienta de trabajo habitual en proyectos de automatización, análisis de datos, ingeniería y desarrollo de software.</p>
<p><strong>📌 Cuadro sinóptico</strong></p>
<ul>
<li><strong>Modularización:</strong> Funciones `def` para evitar la repetición de código.</li>
<li><strong>Git y GitHub:</strong> Git registra el historial local de cambios; GitHub permite alojar y colaborar en repositorios remotos.</li>
</ul>
<p><strong>🧮 Ejemplo conceptual paso a paso</strong></p>
<p><strong>Enunciado:</strong> Definir una función que calcule el promedio de una lista de números.</p>
<pre><code class="language-python">def calcular_promedio(numeros):
    suma_total = sum(numeros)
    cantidad = len(numeros)
    return suma_total / cantidad

resultado = calcular_promedio([10, 20, 30])
print(resultado)
</code></pre>
<p><strong>✏️ Practicá</strong></p>
<p>Indicar qué herramienta se utiliza para guardar el historial local de cambios en un proyecto de código antes de subirlo a GitHub.</p>
<p><strong>✅ Solución:</strong> Git.</p>
</section><section id="formulario" class="module module-formulario"><h2>📑 Hoja de Constantes y Formulario Unificado</h2>
<p>Compendio unificado de fórmulas, constantes universales y ecuaciones clave para consulta durante la resolución de ejercicios.</p>
<p>| <strong>MateriaConcepto / MagnitudFórmula / Valor Universal</strong> |                                  |                                                                                                                           |
| ------------------------------------------------------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| <strong>Química</strong>                                             | Número de Avogadro ($N_A$)      | $N_A = 6.022 \times 10^{23}\text{ partículas/mol}$                                                                       |
| <strong>Química</strong>                                             | Molaridad ($M$) / pH             | $M = \frac{\text{moles de soluto}}{\text{litros de solución}} \quad \vert{} \quad pH = -\log[H^+]$                        |
| <strong>Física</strong>                                              | Aceleración de la gravedad ($g$) | $g \approx 9.8\text{ m/s}^2$                                                                                              |
| <strong>Física</strong>                                              | Presión Hidrostática Absoluta    | $P = P_0 + \rho \cdot g \cdot h$                                                                                         |
| <strong>Física</strong>                                              | Empuje de Arquímedes             | $E = \rho_{fluido} \cdot g \cdot V_{desalojado}$                                                                        |
| <strong>Física</strong>                                              | Ley de Poiseuille (Caudal)       | $Q = \frac{\pi \cdot \Delta P \cdot r^4}{8 \cdot \eta \cdot L} \quad (Q \propto r^4)$                                     |
| <strong>Matemática</strong>                                          | Resolvente Cuadrática            | $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$                                                                                  |
| <strong>Matemática</strong>                                          | Derivada / Integral              | $f'(x) = \text{Pendiente tangente / Tasa de cambio} \quad \vert{} \quad \int_{a}^{b} f(x)dx = \text{Área bajo la curva}$ |</p>
</section>
<footer>Cuadernillo General · contenido organizado para estudiar, consultar y practicar.</footer>
</div>
</body></html>
