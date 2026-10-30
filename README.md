<div align="center">

<a href="https://mglabs.live">
  <img src="./assets/board.svg" width="100%" alt="Tablero de salidas animado: Miguel Molina, backend y full stack, con cinco proyectos">
</a>

<a href="https://mglabs.live">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=19&duration=2600&pause=900&color=6CB4FF&center=true&vCenter=true&width=760&lines=Dise%C3%B1o+APIs+que+aguantan+datos+reales;Arquitectura+hexagonal+%2B+640%2B+pruebas+en+CI;Pedidos+en+vivo+con+Socket.IO+para+un+restaurante+real;Abierto+a+pr%C3%A1cticas+y+primer+rol+backend+%2F+full+stack" alt="Frases animadas">
</a>

<p>
  <a href="https://mglabs.live"><img src="https://img.shields.io/badge/Portafolio-mglabs.live-1554b8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portafolio"></a>
  <a href="https://www.linkedin.com/in/miguel-molina-ab3344394/"><img src="https://img.shields.io/badge/LinkedIn-Conectemos-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:mm6035673@icloud.com"><img src="https://img.shields.io/badge/Correo-Escr%C3%ADbeme-141517?style=for-the-badge&logo=icloud&logoColor=white" alt="Correo"></a>
  <img src="https://komarev.com/ghpvc/?username=MiguelU-coder&style=for-the-badge&color=34c06f&label=VISITAS" alt="Visitas al perfil">
</p>

</div>

## 🎫 Pase de abordar

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/pass-dark.svg">
  <img src="./assets/pass-light.svg" width="100%" alt="Pase de abordar: Miguel Molina, Ingeniería de Software en la Fundación Universitaria Compensar, 4.º de 10 semestres, graduación 2030">
</picture>

Estudio Ingeniería de Software y hago mis prácticas construyendo un sistema que usa un restaurante real todos los días. Lo que más me interesa es el **backend**: reglas de negocio claras, APIs que no pierden ni duplican datos y pruebas que lo demuestran.

## 🟢 Vuelo principal · MM-01 Crocky

<a href="https://mglabs.live/proyectos/crocky">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/crocky-dark.svg">
    <img src="./assets/crocky-light.svg" width="100%" alt="Crocky: cuatro canales de pedido entran a un backend hexagonal y salen a cocina y caja en vivo">
  </picture>
</a>

Sistema de pedidos para **Croky cocina experimental** (Bogotá). El cliente pide desde el QR de su mesa, el kiosko, WhatsApp o el mostrador, y todo cae en vivo a la misma cocina y caja. El repositorio es privado: el caso completo está en **[mglabs.live/proyectos/crocky](https://mglabs.live/proyectos/crocky)**.

<details>
<summary><b>🔍 Ver capturas reales</b></summary>
<br>

<img src="./assets/shots/panel-cocina-wide.webp" width="100%" alt="Panel de cocina de Crocky con pedidos en vivo">

<table>
  <tr>
    <td width="50%"><img src="./assets/shots/pwa-menu.webp" alt="PWA de clientes: menú"></td>
    <td width="50%"><img src="./assets/shots/kiosko.webp" alt="Kiosko en iPad"></td>
  </tr>
  <tr>
    <td align="center"><sub>PWA de clientes (React 19 + Redux Toolkit)</sub></td>
    <td align="center"><sub>Kiosko de caja en iPad</sub></td>
  </tr>
</table>
</details>

<details>
<summary><b>⚙️ Decisiones técnicas que tomé</b></summary>
<br>

| Problema | Cómo lo resolví |
| --- | --- |
| Que el dominio no dependa del framework | Arquitectura hexagonal: 15 puertos, el dominio no conoce Express ni Prisma |
| Pedidos duplicados por mala señal | Idempotencia por `requestId` y cola offline en la PWA |
| Sesiones robadas | Refresh tokens opacos (hash SHA-256), de un solo uso y revocación de toda la familia ante reuso |
| Permisos | Roles `OWNER`, `KITCHEN` y `DELIVERY_DRIVER` verificados contra la BD en cada petición |
| Tarifas de domicilio manipulables | Calculadas en el servidor por zonas de distancia (haversine) |
| Cocina sin refrescar | Socket.IO con respaldo por sondeo |
| Confianza para desplegar | 632 casos Vitest + 14 escenarios Playwright E2E en GitHub Actions |
| Operación | Docker Compose, 37 migraciones Prisma, Grafana + Alloy y automatizaciones con n8n |

</details>

## 🛫 Otros vuelos

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/MiguelU-coder/Bingo-Virtual"><img src="./assets/shots/BingoVirtual.webp" alt="Bingo Virtual"></a>
      <h3><code>MM-02</code> Bingo Virtual</h3>
      Bingo multijugador en tiempo real para hasta 100 jugadores, con resultados auditables mediante SHA-256 y máquina de balotas en 3D.
      <br><br>
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white">
      <img src="https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white">
      <img src="https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61dafb">
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/MiguelU-coder/E-Commerce-MicroServ"><img src="./assets/shots/EcommerceProject.webp" alt="E-commerce con microservicios"></a>
      <h3><code>MM-03</code> E-commerce</h3>
      Tienda en línea con microservicios independientes (auth, pagos, catálogo, pedidos), JWT y panel administrativo.
      <br><br>
      <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white">
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white">
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://github.com/MiguelU-coder/world-cup-crown"><img src="./assets/shots/PollaMundialista.webp" alt="Polla Mundialista"></a>
      <h3><code>MM-04</code> Polla Mundialista</h3>
      Ligas privadas para pronosticar el Mundial, con puntuación automática y tabla de posiciones.
      <br><br>
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white">
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white">
    </td>
    <td width="50%" valign="top">
      <a href="https://github.com/Nikollg205/Sistema_De_Gestion_Para_Farmacias"><img src="./assets/shots/FarmaciaProject.webp" alt="Sistema de Gestión de Farmacia"></a>
      <h3><code>MM-05</code> Farmacia</h3>
      Escritorio para inventario, ventas y reportes, con roles y arquitectura por capas (Singleton + DAO).
      <br><br>
      <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white">
      <img src="https://img.shields.io/badge/Swing-5382A1?style=flat-square">
      <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white">
    </td>
  </tr>
</table>

## 🧰 Stack con evidencia

<div align="center">

| Área | Herramientas |
| :---: | :---: |
| **Lenguajes** | <img src="https://skillicons.dev/icons?i=ts,js,nodejs,java&theme=dark" alt="TypeScript, JavaScript, Node.js, Java"> |
| **Backend y datos** | <img src="https://skillicons.dev/icons?i=express,prisma,postgres,mongodb,mysql&theme=dark" alt="Express, Prisma, PostgreSQL, MongoDB, MySQL"> |
| **Frontend** | <img src="https://skillicons.dev/icons?i=react,nextjs,redux,tailwind&theme=dark" alt="React, Next.js, Redux, Tailwind"> |
| **Calidad y operación** | <img src="https://skillicons.dev/icons?i=vitest,docker,githubactions,grafana,git,linux&theme=dark" alt="Vitest, Docker, GitHub Actions, Grafana, Git, Linux"> |

</div>

## 📊 Actividad

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=MiguelU-coder&show_icons=true&hide_border=true&include_all_commits=true&count_private=true&bg_color=0c0d0e&title_color=6cb4ff&icon_color=34c06f&text_color=f1ede2&border_radius=14&locale=es" alt="Estadísticas de GitHub">
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MiguelU-coder&layout=compact&hide_border=true&bg_color=0c0d0e&title_color=6cb4ff&text_color=f1ede2&border_radius=14&locale=es&langs_count=6" alt="Lenguajes más usados">

<img src="https://streak-stats.demolab.com?user=MiguelU-coder&hide_border=true&background=0C0D0E&ring=1554B8&fire=34C06F&currStreakNum=F1EDE2&sideNums=F1EDE2&currStreakLabel=6CB4FF&sideLabels=8F8D86&dates=8F8D86&border_radius=14&locale=es" alt="Racha de contribuciones">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MiguelU-coder/MiguelU-coder/output/snake-dark.svg">
  <img src="https://raw.githubusercontent.com/MiguelU-coder/MiguelU-coder/output/snake.svg" alt="Serpiente comiéndose el gráfico de contribuciones">
</picture>

</div>

<details>
<summary><b>📜 Certificaciones</b></summary>
<br>

| Año | Certificación |
| :---: | --- |
| 2026 | Hacking ético y ciberseguridad (Kali Linux) |
| 2025 | Node.js Complete Guide: APIs REST, autenticación, MongoDB, SQL y GraphQL |
| 2025 | Full-Stack Web Development Bootcamp: React, Node.js, PostgreSQL y Git |
| 2025 | Certificación avanzada de JavaScript: ES6+, POO, asincronía y código limpio |

</details>

---

<div align="center">

### ¿Tienes una vacante o un proyecto?

<a href="https://mglabs.live/#contact"><img src="https://img.shields.io/badge/Hablemos-mglabs.live-1554b8?style=for-the-badge" alt="Contacto"></a>

<sub>Este perfil sigue el tablero de salidas de <a href="https://mglabs.live">mi portafolio</a>. Las animaciones son SVG hechos a mano.</sub>

</div>
