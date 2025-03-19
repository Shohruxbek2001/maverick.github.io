---
title: "Студент"
date: 2025-03-19T08:47:11+03:00
draft: false
---

{{ define "main" }}

<header>
  <h1>Добро пожаловать в проект!</h1>
  <p>Этот сайт создан с использованием Hugo и темы Terminal.</p>
</header>

<main>
  <section>
    <h2>О проекте</h2>
    <p>Этот проект разработан для демонстрации возможностей Hugo и кастомизации темы Terminal.</p>
    <ul>
      <li><strong>Название:</strong> {{ .Site.Title }}</li>
      <li><strong>Описание:</strong> {{ .Site.Params.description }}</li>
      <li><strong>Версия:</strong> 1.0.0</li>
      <li><strong>Автор:</strong> {{ .Site.Params.author }}</li>
    </ul>
  </section>

  <section>
    <h2>Установка</h2>
    <p>Следуйте этим простым шагам, чтобы развернуть проект на вашем устройстве:</p>
    <pre><code>
git clone https://github.com/your-repo.git
cd your-repo
hugo server
    </code></pre>
  </section>

  <section>
    <h2>Использование</h2>
    <p>Запустите локальный сервер для предпросмотра:</p>
    <pre><code>
hugo server
    </code></pre>
    <p>После этого откройте <a href="http://localhost:1313">http://localhost:1313</a> в браузере.</p>
  </section>
</main>

<footer>
  <p>&copy; {{ now.Year }} {{ .Site.Params.author }}. Все права защищены.</p>
  <p>Создано с ❤️ на Hugo.</p>
</footer>

{{ end }}
