# URL Shortener (Go)

![Go Version](https://img.shields.io/badge/Go-1.25+-00ADD8?logo=go&logoColor=white)
![Built with Go](https://img.shields.io/badge/Built%20with-Go-00ADD8?logo=go&logoColor=white)

A minimal URL shortener API written in Go using `chi`.

## Start the project

1. Install Go `1.25+`.
2. Install dependencies:

```bash
go mod tidy
```

3. Run the server:

```bash
go run .
```

The API starts on `http://localhost:8080`.

## Quick API usage

Create a short code:

```bash
curl -X POST http://localhost:8080/api/shorten \
  -H "Content-Type: application/json" \
  -d '{"url":"https://go.dev"}'
```

Then open:

```text
http://localhost:8080/{code}
```

Replace `{code}` with the value returned by the POST response.
