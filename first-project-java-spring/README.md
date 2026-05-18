# Task 1 - First Spring Boot Project

## How to run
1. Open in IntelliJ IDEA
2. Run `FirstProjectJavaSpringApplication.java`
3. Open browser at `http://localhost:8080`

## Technologies
- Java 17
- Spring Boot 3.2.5
- Thymeleaf
- Lombok

## Endpoints

| Method | URL | Description |
|--------|-----|-------------|
| GET | / | Returns plain text via @ResponseBody |
| GET | /greeting | Returns HTML view via Thymeleaf |
| GET | /greeting?name=Vistula | Returns personalized greeting |

## Screenshots

### GET / — Plain text response
![Hello endpoint](screenshots/hello.png)

### GET /greeting?name=Vistula — HTML view with image
![Greeting endpoint](screenshots/greeting.png)

## How it works
- `@ResponseBody` returns plain text directly to HTTP response
- `@Controller` with Thymeleaf returns HTML views
- `Model` passes data from controller to HTML template
- Image served from `static/images/vistula.png`