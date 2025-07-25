
# 📦 Fundamentos de DevOps

Este proyecto es un sitio web estático generado con [Zola](https://www.getzola.org/), diseñado para enseñar e ilustrar conceptos clave sobre **DevOps**, incluyendo integración continua, automatización, cloud computing y cultura ágil.

## 🌐 Descripción

El sitio proporciona una documentación organizada para un curso/taller de DevOps. Usa Zola como generador estático de sitios y está preparado para desarrollo y despliegue con Docker.

## 📁 Estructura del Proyecto

- `Dockerfile` – Construye el sitio usando Zola y lo sirve con un servidor web estático.
- `Dockerfile.dev` – Imagen para desarrollo local que incluye `zola serve`.
- `docker-compose.yml` – Orquesta el entorno de desarrollo con sincronización automática.
- `config.toml` – Configuración del sitio Zola (título, idioma, tema, rutas, SEO, etc).
- `.gitmodules` – Indica posibles temas externos usados como submódulos Git.

## 🚀 Cómo usar

### 1. Clonar el proyecto

```bash
git clone https://github.com/tuusuario/devops-fundamentals.git
cd devops-fundamentals
```

### 2. Desarrollar localmente

```bash
docker-compose up
```

Luego abre en tu navegador: [http://localhost:1111](http://localhost:1111)

### 3. Generar sitio para producción

```bash
docker build -t devops-site .
docker run -p 8080:80 devops-site
```

Luego accede a: [http://localhost:8080](http://localhost:8080)

## 🛠 Tecnologías

- [Zola v0.17.1](https://github.com/getzola/zola)
- Docker / Docker Compose
- HTML estático
- Tema Zola: `adidoks`

## 👤 Autor

- **Sebastián Jiménez**  
- Sitio generado como parte del curso: *Fundamentos de DevOps*

## 📝 Licencia

Este proyecto está bajo la licencia MIT.