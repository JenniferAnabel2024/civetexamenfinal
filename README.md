# CIVET - Terminal Veterinario (Versión Clásica)

Bienvenido al proyecto **CIVET**, una aplicación web para la gestión de una terminal veterinaria. Esta versión clásica está desarrollada con tecnologías modernas pero manteniendo una interfaz simple y funcional.

## 🚀 Tecnologías Utilizadas

- **Backend:** Spring Boot 3.4.5 con Java 21
- **Base de Datos:** MySQL con JPA/Hibernate
- **Frontend:** HTML5, CSS3, JavaScript (jQuery + Bootstrap 5)
- **Build Tool:** Maven
- **Version Control:** Git

## 📋 Características

### Módulos Disponibles
- **Inicio:** Página de bienvenida con información general
- **Quienes Somos:** Información sobre la clínica veterinaria
- **Turnos:** Gestión completa de citas veterinarias (CRUD)
  - Crear nuevos turnos
  - Ver turnos programados
  - Editar turnos existentes
  - Eliminar turnos
- **Pacientes:** Gestión de mascotas
- **Ficha Paciente:** Registros médicos
- **Tienda:** Catálogo de productos
- **Contacto:** Información de contacto

### Funcionalidades Técnicas
- API RESTful para todas las operaciones
- Interfaz responsive con Bootstrap
- Validación de formularios
- Manejo de errores robusto
- Base de datos relacional con MySQL

## 🛠️ Instalación y Ejecución

### Prerrequisitos
- Java 21 (JDK)
- Maven 3.9+
- MySQL 8.0+
- Git

### Pasos de Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/JenniferAnabel2024/civetclasic.git
   cd civetclasic
   ```

2. **Configurar la base de datos:**
   - Crear una base de datos MySQL llamada `civetdb`
   - Ejecutar los scripts SQL en `src/main/resources/sql/`:
     - `schema-mysql.sql` (crea las tablas)
     - `data-mysql.sql` (inserta datos de prueba)

3. **Configurar la conexión a BD:**
   Editar `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/civetdb
   spring.datasource.username=tu_usuario
   spring.datasource.password=tu_password
   spring.jpa.hibernate.ddl-auto=update
   ```

4. **Ejecutar la aplicación:**
   ```bash
   mvn spring-boot:run
   ```

5. **Acceder a la aplicación:**
   Abrir en el navegador: `http://localhost:8080`

## 📁 Estructura del Proyecto

```
civetclasic/
├── src/main/java/com/civet/backend/
│   ├── entity/          # Entidades JPA
│   ├── repo/            # Repositorios
│   ├── service/         # Servicios de negocio
│   └── web/             # Controladores REST
├── src/main/resources/
│   ├── sql/             # Scripts de BD
│   ├── static/          # Frontend (HTML, CSS, JS)
│   └── application.properties
├── estructura_civerweb.md  # Documentación técnica
└── pom.xml              # Configuración Maven
```

## 🔧 API Endpoints

### Turnos
- `GET /api/turnos` - Listar todos los turnos
- `GET /api/turnos/{id}` - Obtener turno por ID
- `POST /api/turnos` - Crear nuevo turno
- `PUT /api/turnos/{id}` - Actualizar turno
- `DELETE /api/turnos/{id}` - Eliminar turno

### Pacientes
- `GET /api/pacientes` - Listar pacientes
- `POST /api/pacientes` - Crear paciente

### Médicos
- `GET /api/medicos` - Listar médicos

### Productos
- `GET /api/productos` - Listar productos tienda

## 🤝 Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -am 'Agrega nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📞 Contacto

**CIVET - Centro Integral Veterinario**
- WhatsApp: [+5492612502161](https://wa.me/5492612502161)
- Email: contacto@civet.com.ar

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

---

*Desarrollado con ❤️ para el cuidado de las mascotas*</content>
<parameter name="filePath">c:\Users\Raulacate\Desktop\Jeny Manuel Belgrano\Proyectos\classic-version\README.md