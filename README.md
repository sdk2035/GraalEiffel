# GraalEiffel 🚀

**GraalEiffel** es una implementación de alto rendimiento del lenguaje de programación **Eiffel**, desarrollada sobre **GraalVM** utilizando el framework Truffle.

Esta plataforma aprovecha los principios de Diseño por Contrato (Design by Contract™) nativos de Eiffel y los combina con la potencia del compilador JIT (Just-In-Time) de GraalVM, permitiendo ejecutar software orientado a objetos altamente confiable con rendimiento de nivel de producción e interoperabilidad políglota.

---

## 🌟 Características Principales

* **Diseño por Contrato Optimizado:** Compilación y verificación eficiente de precondiciones, poscondiciones e invariantes de clase sin penalizaciones de rendimiento en producción.
* **Rendimiento de Alto Nivel (GraalVM JIT):** Optimizaciones dinámicas avanzadas (inlining de llamadas a métodos, *escape analysis*) sobre el AST de Truffle.
* **Ecosistema Políglota:** Integración nativa e intercambio de objetos sin fricción con Java, Python, JavaScript, Ruby y otros lenguajes soportados por GraalVM.
* **Compilación Nativa (Native Image):** Generación de binarios autónomos y ligeros con **GraalVM Native Image** para despliegues rápidos en la nube y contenedores.

---

## 🏗️ Arquitectura de la Plataforma

* **Eiffel Truffle Parser:** Transforma el código fuente Eiffel en un árbol de sintaxis abstracta (AST) optimizado para el motor Truffle.
* **Contract Enforcement Engine:** Mecanismo especializado dentro del runtime para la evaluación eficiente de contratos de software en tiempo de ejecución.
* **GraalVM JIT Compiler:** Motor que compila en tiempo de ejecución los nodos de AST más frecuentados (*hot spots*) a código máquina altamente optimizado.

---

## 🚦 Inicio Rápido

### Prerrequisitos

* **GraalVM JDK** (versión 21 o superior) con componentes de Truffle habilitados.
* Variable de entorno `JAVA_HOME` apuntando al directorio de GraalVM.

### Instalación

```bash
# Clonar el repositorio
git clone [https://github.com/tu-usuario/graaleiffel.git](https://github.com/tu-usuario/graaleiffel.git)
cd graaleiffel

# Construir el proyecto utilizando Gradle
./gradlew build
