# Estructura HTML de la Landing Page - VisionTranslate

He diseñado la estructura HTML de la landing page priorizando la semántica correcta para mejorar el SEO, la accesibilidad y la organización lógica del contenido.

---

## Header y Navegación Principal

```html
<header role="banner">
    <nav class="main-nav" aria-label="Navegación principal">
        <a href="#" class="logo">VisionTranslate</a>
        <ul>...</ul>
        <aside class="user-controls">...</aside>
    </nav>
</header>
```

**Justificación:**

- `<header>`: Representa el encabezado introductorio de la página. Se complementa con `role="banner"` para mejorar la accesibilidad.
- `<nav>`: Utilizado para la navegación principal con `aria-label` para identificarla claramente para lectores de pantalla.
- `<aside>`: Contiene los controles de usuario (búsqueda y carrito) que están relacionados con la navegación pero son complementarios.

---

## Sección Hero

```html
<section id="hero" aria-labelledby="hero-heading">
    <article class="hero-content">
        <h1 id="hero-heading">Los Nuevos Lentes VisionTranslate</h1>
        <p class="tagline">...</p>
        <nav class="cta-nav">...</nav>
        <figure class="hero-image">...</figure>
    </article>
</section>
```

**Justificación:**

- `<section>`: Define una sección temática específica con su propio encabezado.
- `aria-labelledby`: Vincula la sección con su encabezado para mejorar la accesibilidad.
- `<article>`: Contiene contenido independiente que tendría sentido fuera del contexto de la página.
- `<h1>`: El encabezado principal de la página.
- `<nav>`: Usado para botones de llamada a la acción.
- `<figure>`: Imagen principal ilustrativa.

---

## Sección de Características

```html
<section id="caracteristicas" aria-labelledby="caracteristicas-heading">
    <h2 id="caracteristicas-heading">Características principales</h2>
    <ul class="features-list">
        <li>
            <article class="feature">...</article>
        </li>
        ...
    </ul>
</section>
```

**Justificación:**

- `<section>`: Sección temática específica.
- `<h2>`: Encabezado de segundo nivel.
- `<ul>` y `<li>`: Lista no ordenada de características.
- `<article>`: Cada característica es un contenido independiente.

---

## Sección de Envío

```html
<section id="envio" aria-labelledby="envio-heading">
    <h2 id="envio-heading">Opciones de envío</h2>
    <article class="shipping-info">
        <section class="shipping-column">...</section>
        <section class="shipping-column">...</section>
    </article>
</section>
```

**Justificación:**

- `<section>`: Sección temática específica.
- `<article>`: Contiene información completa sobre envío.
- `<section>` dentro de `<article>`: Subgrupos temáticos.

---

## Sección de Pagos

```html
<section id="pagos" aria-labelledby="pagos-heading">
    <h2 id="pagos-heading">Métodos de pago</h2>
    <ul class="payment-methods">
        <li>Tarjetas de crédito</li>
        ...
    </ul>
</section>
```

**Justificación:**

- `<section>`: Sección temática específica.
- `<ul>` y `<li>`: Lista de métodos de pago.

---

## Footer

```html
<footer id="contacto" role="contentinfo">
    <section class="footer-sections">
        <article class="contact-info">
            <h3>Contacto</h3>
            <address>...</address>
        </article>
        <nav class="footer-links" aria-label="Enlaces importantes">...</nav>
        <aside class="social-section">...</aside>
    </section>
    <small class="copyright">...</small>
</footer>
```

**Justificación:**

- `<footer>`: Pie de página con `role="contentinfo"`.
- `<article>`: Información de contacto.
- `<address>`: Información de contacto.
- `<nav>`: Enlaces importantes.
- `<aside>`: Redes sociales.
- `<small>`: Copyright.

---

## Beneficios de esta estructura

- **Mejora del SEO**: Uso correcto de etiquetas semánticas.
- **Mantenibilidad**: Código organizado y fácil de entender.
- **Compatibilidad futura**: Basado en HTML5 y buenas prácticas.
- **Consistencia**: Jerarquía de encabezados clara (h1 > h2 > h3).
