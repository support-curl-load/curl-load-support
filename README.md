# curl-load Support

Welcome to the support repository for **curl-load** 🚀

Use this repo to:
- 🐛 Report bugs
- 💡 Request features
- ❓ Ask questions

---

## 🚀 Getting Started

The easiest way to run curl-load is via Docker.

### 📦 Prerequisites

- Install Docker: https://docs.docker.com/get-docker/

Verify installation:

```bash
docker --version
```

---

## ▶️ Run curl-load

```bash
docker run -p 3000:3000 -p 5665:5665 -v curl-load-runs:/app/runs curlload/curl-load-runner:latest
```

---

## 🌐 Access the Workbench

Once the container is running, open:

http://localhost:3000/load-tester.html

This is the **curl-load Workbench**, where you can:
- Paste curl commands
- Configure load tests
- Run tests locally or remotely

---

## 🔌 Ports

| Port | Description |
|------|------------|
| 3000 | Web UI (Workbench) |
| 5665 | Remote runner / execution API |

---

## 🧪 Example Usage

1. Open the Workbench
2. Paste a curl command:

```bash
curl -X GET "https://api.example.com/data?limit=10"
```

3. Configure:
    - Virtual Users
    - Duration or Iterations
    - Variables (optional)

4. Click **Run Test**

---

## 🐛 Reporting Issues

When reporting a bug, please include:

- curl command used
- configuration (VUs, duration, etc.)
- expected vs actual behavior
- screenshots (if applicable)

---

## 💡 Feature Requests

We welcome ideas! Please include:
- problem you're trying to solve
- proposed solution
- example use case

---

## 📌 Notes

- Docker is required to run the backend runner
- Some APIs may block browser requests due to CORS
- For best results, run tests against APIs that allow direct access

---

## 🔗 Links

- Workbench: http://localhost:3000/load-tester.html
- Dashboard: http://localhost:3000/
- Documentation: http://localhost:3000/documentation.html

---

## 🧠 About curl-load

curl-load is a lightweight load testing tool that lets you:
- Use existing curl commands
- Run load tests instantly
- Avoid complex setup

---

## ⭐ Contributing

Feel free to open issues or suggestions — feedback is highly appreciated!
